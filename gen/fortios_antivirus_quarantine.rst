:source: fortios_antivirus_quarantine.py

:orphan:

.. _fortios_antivirus_quarantine:

fortios_antivirus_quarantine -- Configure quarantine options in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify antivirus feature and quarantine category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">antivirus_quarantine</span> - Configure quarantine options. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">agelimit</span> - Age limit for quarantined files (0 - 479 hours, 0 means forever). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">destination</span> - Choose whether to quarantine files to the FortiGate disk or to FortiAnalyzer or to delete them instead of quarantining them. <span class="li-normal">type: str</span> <span class="li-normal">choices: NULL,  disk,  FortiAnalyzer</span></li>
            <li><span class="li-head">drop_blocked</span> - Do not quarantine dropped files found in sessions using the selected protocols. Dropped files are deleted instead of being quarantined. <span class="li-normal">type: str</span> <span class="li-normal">choices: imap,  smtp,  pop3,  http,  ftp,  nntp,  imaps,  smtps,  pop3s,  ftps,  mapi,  cifs,  mm1,  mm3,  mm4,  mm7</span></li>
            <li><span class="li-head">drop_heuristic</span> - Do not quarantine files detected by heuristics found in sessions using the selected protocols. Dropped files are deleted instead of being quarantined. <span class="li-normal">type: str</span> <span class="li-normal">choices: imap,  smtp,  pop3,  http,  ftp,  nntp,  imaps,  smtps,  pop3s,  https,  ftps,  mapi,  cifs,  mm1,  mm3,  mm4,  mm7</span></li>
            <li><span class="li-head">drop_infected</span> - Do not quarantine infected files found in sessions using the selected protocols. Dropped files are deleted instead of being quarantined. <span class="li-normal">type: str</span> <span class="li-normal">choices: imap,  smtp,  pop3,  http,  ftp,  nntp,  imaps,  smtps,  pop3s,  https,  ftps,  mapi,  cifs,  mm1,  mm3,  mm4,  mm7</span></li>
            <li><span class="li-head">lowspace</span> - Select the method for handling additional files when running low on disk space. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop-new,  ovrw-old</span></li>
            <li><span class="li-head">maxfilesize</span> - Maximum file size to quarantine (0 - 500 Mbytes, 0 means unlimited). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">quarantine_quota</span> - The amount of disk space to reserve for quarantining files (0 - 4294967295 Mbytes, depends on disk space). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">store_blocked</span> - Quarantine blocked files found in sessions using the selected protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: imap,  smtp,  pop3,  http,  ftp,  nntp,  imaps,  smtps,  pop3s,  ftps,  mapi,  cifs,  mm1,  mm3,  mm4,  mm7</span></li>
            <li><span class="li-head">store_heuristic</span> - Quarantine files detected by heuristics found in sessions using the selected protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: imap,  smtp,  pop3,  http,  ftp,  nntp,  imaps,  smtps,  pop3s,  https,  ftps,  mapi,  cifs,  mm1,  mm3,  mm4,  mm7</span></li>
            <li><span class="li-head">store_infected</span> - Quarantine infected files found in sessions using the selected protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: imap,  smtp,  pop3,  http,  ftp,  nntp,  imaps,  smtps,  pop3s,  https,  ftps,  mapi,  cifs,  mm1,  mm3,  mm4,  mm7</span>
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
      - name: Configure quarantine options.
        fortios_antivirus_quarantine:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          antivirus_quarantine:
            agelimit: "3"
            destination: "NULL"
            drop_blocked: "imap"
            drop_heuristic: "imap"
            drop_infected: "imap"
            lowspace: "drop-new"
            maxfilesize: "9"
            quarantine_quota: "10"
            store_blocked: "imap"
            store_heuristic: "imap"
            store_infected: "imap"



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