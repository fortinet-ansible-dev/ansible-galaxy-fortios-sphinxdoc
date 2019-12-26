:source: fortios_webfilter.py

:orphan:

.. _fortios_webfilter:

fortios_webfilter -- Configure webfilter capabilities of FortiGate and FortiOS.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.6

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS by allowing the user to configure webfilter feature. For now it is able to handle url and content filtering capabilities. The module uses FortiGate REST API internally to configure the device.


Requirements
------------
The below requirements are needed on the host that executes this module.

- fortiosapi>=0.9.8


Parameters
----------

.. raw:: html

    <ul>

    <li><span class="li-head">host</span> - FortiOS or FortiGate ip address. <span class="li-required">required</span></li>
    <li><span class="li-head">username</span> - FortiOS or FortiGate username. <span class="li-required">required</span></li>
    <li><span class="li-head">password</span> - FortiOS or FortiGate password. <span class="li-normal">default: ""</span></li>
    <li><span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">default: "root"</span></li>
    <li><span class="li-head">webfilter_url</span> - Container for a group of url entries that the FortiGate must act upon</li>
            <ul class="ul-self">

            <li><span class="li-head">id</span> - Id of URL filter list. <span class="li-required">required</span></li>
            <li><span class="li-head">name</span> - Name of URL filter list. <span class="li-required">required</span></li>
            <li><span class="li-head">comment</span> - Optional comments.</li>
            <li><span class="li-head">one-arm-ips-urlfilter</span> - Enable/disable DNS resolver for one-arm IPS URL filter operation. <span class="li-normal">choices: enable,  disable</span> <span class="li-normal">default: disable</span></li>
            <li><span class="li-head">ip-addr-block</span> - Enable/disable blocking URLs when the hostname appears as an IP address. <span class="li-normal">choices: enable,  disable</span> <span class="li-normal">default: disable</span></li>
            <li><span class="li-head">entries</span> - URL filter entries. <span class="li-normal">default: []</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - Id of URL. <span class="li-required">required</span></li>
                    <li><span class="li-head">url</span> - URL to be filtered. <span class="li-required">required</span> <span class="li-normal">type:</span> Filter type (simple, regex, or wildcard). <span class="li-required">required</span> <span class="li-normal">choices: simple,  regex,  wildcard</span></li>
                    <li><span class="li-head">action</span> - Action to take for URL filter matches. <span class="li-required">required</span> <span class="li-normal">choices: exempt,  block,  allow,  monitor</span></li>
                    <li><span class="li-head">status</span> - Enable/disable this URL filter. <span class="li-required">required</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">exempt</span> - If action is set to exempt, select the security profile operations that exempt URLs skip. Separate multiple options with a space. <span class="li-required">required</span> <span class="li-normal">choices: av,  web-content,  activex-java-cookie,  dlp,  fortiguard,  range-block,  pass,  all</span></li>
                    <li><span class="li-head">web-proxy-profile</span> - Web proxy profile. <span class="li-required">required</span></li>
                    <li><span class="li-head">referrer-host</span> - Referrer host name. <span class="li-required">required</span>
                    </ul>

            <li><span class="li-head">state</span> - Configures the intended state of this object on the FortiGate. When this value is set to I(present), the object is configured on the device and when this value is set to I(absent) the object is removed from the device. <span class="li-required">required</span> <span class="li-normal">choices: absent,  present</span>
            </ul>

    <li><span class="li-head">webfilter_content</span> - Container for a group of content-filtering entries that the FortiGate must act upon</li>
            <ul class="ul-self">

            <li><span class="li-head">id</span> - Id of content-filter list. <span class="li-required">required</span></li>
            <li><span class="li-head">name</span> - Name of content-filter list.</li>
            <li><span class="li-head">comment</span> - Optional comments.</li>
            <li><span class="li-head">entries</span> - Content filter entries. <span class="li-normal">default: []</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Banned word. <span class="li-required">required</span></li>
                    <li><span class="li-head">pattern-type</span> - Banned word pattern type. It can be a wildcard pattern or Perl regular expression. <span class="li-required">required</span> <span class="li-normal">choices: wildcard,  regexp</span></li>
                    <li><span class="li-head">status</span> - Enable/disable banned word. <span class="li-required">required</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">lang</span> - Language of banned word. <span class="li-required">required</span> <span class="li-normal">choices: western,  simch,  trach,  japanese,  korean,  french,  thai,  spanish,  cyrillic</span></li>
                    <li><span class="li-head">score</span> - Score, to be applied every time the word appears on a web page. <span class="li-required">required</span></li>
                    <li><span class="li-head">action</span> - Block or exempt word when a match is found. <span class="li-required">required</span> <span class="li-normal">choices: block,  exempt</span>
                    </ul>

            <li><span class="li-head">state</span> - Configures the intended state of this object on the FortiGate. When this value is set to I(present), the object is configured on the device and when this value is set to I(absent) the object is removed from the device. <span class="li-required">required</span> <span class="li-normal">choices: absent,  present</span>
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
      tasks:
      - name: Configure url to be filtered by fortigate
        fortios_webfilter:
          host:  "{{  host }}"
          username: "{{  username}}"
          password: "{{ password }}"
          vdom:  "{{  vdom }}"
          webfilter_url:
            state: "present"
            id: "1"
            name: "default"
            comment: "mycomment"
            one-arm-ips-url-filter: "disable"
            ip-addr-block: "disable"
            entries:
              - id: "1"
                url: "www.test1.com"
                type: "simple"
                action: "exempt"
                status: "enable"
                exempt: "pass"
                web-proxy-profile: ""
                referrrer-host: ""
              - id: "2"
                url: "www.test2.com"
                type: "simple"
                action: "exempt"
                status: "enable"
                exempt: "pass"
                web-proxy-profile: ""
                referrrer-host: ""


    - hosts: localhost
      vars:
       host: "192.168.122.40"
       username: "admin"
       password: ""
       vdom: "root"
      tasks:
      - name: Configure web content filtering in fortigate
        fortios_webfilter:
          host:  "{{  host }}"
          username: "{{  username}}"
          password: "{{ password }}"
          vdom:  "{{  vdom }}"
          webfilter_content:
            id: "1"
            name: "default"
            comment: ""
            entries:
              - name: "1"
                pattern-type: "www.test45.com"
                status: "enable"
                lang: "western"
                score: 40
                action: "block"
              - name: "2"
                pattern-type: "www.test46.com"
                status: "enable"
                lang: "western"
                score: 42
                action: "block"
            state: "present"



Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: '1547'</span></li>
    <li><span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 'PUT'</span></li>
    <li><span class="li-return">http_status</span> - Last result given by FortiGate on last operation applied <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 200</span></li>
    <li><span class="li-return">mkey</span> - Master key (id) used in the last call to FortiGate <span class="li-normal">returned: success</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: key1</span></li>
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