:source: fortios_antivirus_profile.py

:orphan:

.. _fortios_antivirus_profile:

fortios_antivirus_profile -- Configure AntiVirus profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify antivirus feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">antivirus_profile</span> - Configure AntiVirus profiles. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">analytics_bl_filetype</span> - Only submit files matching this DLP file-pattern to FortiSandbox. Source dlp.filepattern.id. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">analytics_db</span> - Enable/disable using the FortiSandbox signature database to supplement the AV signature databases. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">analytics_max_upload</span> - Maximum size of files that can be uploaded to FortiSandbox (1 - 395 MBytes). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">analytics_wl_filetype</span> - Do not submit files matching this DLP file-pattern to FortiSandbox. Source dlp.filepattern.id. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">av_block_log</span> - Enable/disable logging for AntiVirus file blocking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">av_virus_log</span> - Enable/disable AntiVirus logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">content_disarm</span> - AV Content Disarm and Reconstruction settings. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">cover_page</span> - Enable/disable inserting a cover page into the disarmed document. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">detect_only</span> - Enable/disable only detect disarmable files, do not alter content. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">office_embed</span> - Enable/disable stripping of embedded objects in Microsoft Office documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">office_hylink</span> - Enable/disable stripping of hyperlinks in Microsoft Office documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">office_linked</span> - Enable/disable stripping of linked objects in Microsoft Office documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">office_macro</span> - Enable/disable stripping of macros in Microsoft Office documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">original_file_destination</span> - Destination to send original file if active content is removed. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortisandbox,  quarantine,  discard</span></li>
                    <li><span class="li-head">pdf_act_form</span> - Enable/disable stripping of actions that submit data to other targets in PDF documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">pdf_act_gotor</span> - Enable/disable stripping of links to other PDFs in PDF documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">pdf_act_java</span> - Enable/disable stripping of actions that execute JavaScript code in PDF documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">pdf_act_launch</span> - Enable/disable stripping of links to external applications in PDF documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">pdf_act_movie</span> - Enable/disable stripping of embedded movies in PDF documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">pdf_act_sound</span> - Enable/disable stripping of embedded sound files in PDF documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">pdf_embedfile</span> - Enable/disable stripping of embedded files in PDF documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">pdf_hyperlink</span> - Enable/disable stripping of hyperlinks from PDF documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">pdf_javacode</span> - Enable/disable stripping of JavaScript code in PDF documents. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span>
                    </ul>

            <li><span class="li-head">extended_log</span> - Enable/disable extended logging for antivirus. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">ftgd_analytics</span> - Settings to control which files are uploaded to FortiSandbox. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  suspicious,  everything</span></li>
            <li><span class="li-head">ftp</span> - Configure FTP AntiVirus options. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">archive_block</span> - Select the archive types to block. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">archive_log</span> - Select the archive types to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">emulator</span> - Enable/disable the virus emulator. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">options</span> - Enable/disable FTP AntiVirus scanning, monitoring, and quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: scan,  avmonitor,  quarantine</span></li>
                    <li><span class="li-head">outbreak_prevention</span> - Enable FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled,  files,  full-archive</span>
                    </ul>

            <li><span class="li-head">http</span> - Configure HTTP AntiVirus options. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">archive_block</span> - Select the archive types to block. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">archive_log</span> - Select the archive types to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">content_disarm</span> - Enable Content Disarm and Reconstruction for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">emulator</span> - Enable/disable the virus emulator. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">options</span> - Enable/disable HTTP AntiVirus scanning, monitoring, and quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: scan,  avmonitor,  quarantine</span></li>
                    <li><span class="li-head">outbreak_prevention</span> - Enable FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled,  files,  full-archive</span>
                    </ul>

            <li><span class="li-head">imap</span> - Configure IMAP AntiVirus options. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">archive_block</span> - Select the archive types to block. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">archive_log</span> - Select the archive types to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">content_disarm</span> - Enable Content Disarm and Reconstruction for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">emulator</span> - Enable/disable the virus emulator. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">executables</span> - Treat Windows executable files as viruses for the purpose of blocking or monitoring. <span class="li-normal">type: str</span> <span class="li-normal">choices: default,  virus</span></li>
                    <li><span class="li-head">options</span> - Enable/disable IMAP AntiVirus scanning, monitoring, and quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: scan,  avmonitor,  quarantine</span></li>
                    <li><span class="li-head">outbreak_prevention</span> - Enable FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled,  files,  full-archive</span>
                    </ul>

            <li><span class="li-head">inspection_mode</span> - Inspection mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: proxy,  flow-based</span></li>
            <li><span class="li-head">mapi</span> - Configure MAPI AntiVirus options. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">archive_block</span> - Select the archive types to block. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">archive_log</span> - Select the archive types to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">emulator</span> - Enable/disable the virus emulator. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">executables</span> - Treat Windows executable files as viruses for the purpose of blocking or monitoring. <span class="li-normal">type: str</span> <span class="li-normal">choices: default,  virus</span></li>
                    <li><span class="li-head">options</span> - Enable/disable MAPI AntiVirus scanning, monitoring, and quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: scan,  avmonitor,  quarantine</span></li>
                    <li><span class="li-head">outbreak_prevention</span> - Enable FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled,  files,  full-archive</span>
                    </ul>

            <li><span class="li-head">mobile_malware_db</span> - Enable/disable using the mobile malware signature database. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">nac_quar</span> - Configure AntiVirus quarantine settings. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">expiry</span> - Duration of quarantine. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">infected</span> - Enable/Disable quarantining infected hosts to the banned user list. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  quar-src-ip</span></li>
                    <li><span class="li-head">log</span> - Enable/disable AntiVirus quarantine logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">name</span> - Profile name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">nntp</span> - Configure NNTP AntiVirus options. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">archive_block</span> - Select the archive types to block. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">archive_log</span> - Select the archive types to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">emulator</span> - Enable/disable the virus emulator. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">options</span> - Enable/disable NNTP AntiVirus scanning, monitoring, and quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: scan,  avmonitor,  quarantine</span></li>
                    <li><span class="li-head">outbreak_prevention</span> - Enable FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled,  files,  full-archive</span>
                    </ul>

            <li><span class="li-head">pop3</span> - Configure POP3 AntiVirus options. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">archive_block</span> - Select the archive types to block. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">archive_log</span> - Select the archive types to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">content_disarm</span> - Enable Content Disarm and Reconstruction for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">emulator</span> - Enable/disable the virus emulator. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">executables</span> - Treat Windows executable files as viruses for the purpose of blocking or monitoring. <span class="li-normal">type: str</span> <span class="li-normal">choices: default,  virus</span></li>
                    <li><span class="li-head">options</span> - Enable/disable POP3 AntiVirus scanning, monitoring, and quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: scan,  avmonitor,  quarantine</span></li>
                    <li><span class="li-head">outbreak_prevention</span> - Enable FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled,  files,  full-archive</span>
                    </ul>

            <li><span class="li-head">replacemsg_group</span> - Replacement message group customized for this profile. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">scan_mode</span> - Choose between full scan mode and quick scan mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: quick,  full</span></li>
            <li><span class="li-head">smb</span> - Configure SMB AntiVirus options. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">archive_block</span> - Select the archive types to block. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">archive_log</span> - Select the archive types to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">emulator</span> - Enable/disable the virus emulator. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">options</span> - Enable/disable SMB AntiVirus scanning, monitoring, and quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: scan,  avmonitor,  quarantine</span></li>
                    <li><span class="li-head">outbreak_prevention</span> - Enable FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled,  files,  full-archive</span>
                    </ul>

            <li><span class="li-head">smtp</span> - Configure SMTP AntiVirus options. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">archive_block</span> - Select the archive types to block. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">archive_log</span> - Select the archive types to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: encrypted,  corrupted,  partiallycorrupted,  multipart,  nested,  mailbomb,  fileslimit,  timeout,  unhandled</span></li>
                    <li><span class="li-head">content_disarm</span> - Enable Content Disarm and Reconstruction for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">emulator</span> - Enable/disable the virus emulator. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">executables</span> - Treat Windows executable files as viruses for the purpose of blocking or monitoring. <span class="li-normal">type: str</span> <span class="li-normal">choices: default,  virus</span></li>
                    <li><span class="li-head">options</span> - Enable/disable SMTP AntiVirus scanning, monitoring, and quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: scan,  avmonitor,  quarantine</span></li>
                    <li><span class="li-head">outbreak_prevention</span> - Enable FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled,  files,  full-archive</span>
                    </ul>

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
      - name: Configure AntiVirus profiles.
        fortios_antivirus_profile:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          antivirus_profile:
            analytics_bl_filetype: "3 (source dlp.filepattern.id)"
            analytics_db: "disable"
            analytics_max_upload: "5"
            analytics_wl_filetype: "6 (source dlp.filepattern.id)"
            av_block_log: "enable"
            av_virus_log: "enable"
            comment: "Comment."
            content_disarm:
                cover_page: "disable"
                detect_only: "disable"
                office_embed: "disable"
                office_hylink: "disable"
                office_linked: "disable"
                office_macro: "disable"
                original_file_destination: "fortisandbox"
                pdf_act_form: "disable"
                pdf_act_gotor: "disable"
                pdf_act_java: "disable"
                pdf_act_launch: "disable"
                pdf_act_movie: "disable"
                pdf_act_sound: "disable"
                pdf_embedfile: "disable"
                pdf_hyperlink: "disable"
                pdf_javacode: "disable"
            extended_log: "enable"
            ftgd_analytics: "disable"
            ftp:
                archive_block: "encrypted"
                archive_log: "encrypted"
                emulator: "enable"
                options: "scan"
                outbreak_prevention: "disabled"
            http:
                archive_block: "encrypted"
                archive_log: "encrypted"
                content_disarm: "disable"
                emulator: "enable"
                options: "scan"
                outbreak_prevention: "disabled"
            imap:
                archive_block: "encrypted"
                archive_log: "encrypted"
                content_disarm: "disable"
                emulator: "enable"
                executables: "default"
                options: "scan"
                outbreak_prevention: "disabled"
            inspection_mode: "proxy"
            mapi:
                archive_block: "encrypted"
                archive_log: "encrypted"
                emulator: "enable"
                executables: "default"
                options: "scan"
                outbreak_prevention: "disabled"
            mobile_malware_db: "disable"
            nac_quar:
                expiry: "<your_own_value>"
                infected: "none"
                log: "enable"
            name: "default_name_63"
            nntp:
                archive_block: "encrypted"
                archive_log: "encrypted"
                emulator: "enable"
                options: "scan"
                outbreak_prevention: "disabled"
            pop3:
                archive_block: "encrypted"
                archive_log: "encrypted"
                content_disarm: "disable"
                emulator: "enable"
                executables: "default"
                options: "scan"
                outbreak_prevention: "disabled"
            replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
            scan_mode: "quick"
            smb:
                archive_block: "encrypted"
                archive_log: "encrypted"
                emulator: "enable"
                options: "scan"
                outbreak_prevention: "disabled"
            smtp:
                archive_block: "encrypted"
                archive_log: "encrypted"
                content_disarm: "disable"
                emulator: "enable"
                executables: "default"
                options: "scan"
                outbreak_prevention: "disabled"



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