:source: fortios_spamfilter_bword.py

:orphan:

.. fortios_spamfilter_bword:

fortios_spamfilter_bword -- Configure AntiSpam banned word list in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify spamfilter feature and bword category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">spamfilter_bword</span> - Configure AntiSpam banned word list. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">comment</span> - Optional comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">entries</span> - Spam filter banned word. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Mark spam or good. <span class="li-normal">type: str</span> <span class="li-normal">choices: spam, clear</span></li>
            <li> <span class="li-head">id</span> - Banned word entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">language</span> - Language for the banned word. <span class="li-normal">type: str</span> <span class="li-normal">choices: western, simch, trach, japanese, korean, french, thai, spanish</span></li>
            <li> <span class="li-head">pattern</span> - Pattern for the banned word. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">pattern_type</span> - Wildcard pattern or regular expression. <span class="li-normal">type: str</span> <span class="li-normal">choices: wildcard, regexp</span></li>
            <li> <span class="li-head">score</span> - Score value. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">where</span> - Component of the email to be scanned. <span class="li-normal">type: str</span> <span class="li-normal">choices: subject, body, all</span></li>
            </ul>
        <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">name</span> - Name of table. <span class="li-normal">type: str</span></li>
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
      - name: Configure AntiSpam banned word list.
        fortios_spamfilter_bword:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          spamfilter_bword:
            comment: "Optional comments."
            entries:
             -
                action: "spam"
                id:  "6"
                language: "western"
                pattern: "<your_own_value>"
                pattern_type: "wildcard"
                score: "10"
                status: "enable"
                where: "subject"
            id:  "13"
            name: "default_name_14"
    


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
