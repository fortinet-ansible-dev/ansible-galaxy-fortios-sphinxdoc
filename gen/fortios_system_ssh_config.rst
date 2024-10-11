:source: fortios_system_ssh_config.py

:orphan:

.. fortios_system_ssh_config:

fortios_system_ssh_config -- Configure SSH config in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and ssh_config category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.4.4 -> v7.6.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">system_ssh_config</span> - Configure SSH config. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_ssh_config</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">ssh_enc_algo</span> - Select one or more SSH ciphers. <span class="li-normal">type: list</span> <span class="li-normal">choices: chacha20-poly1305@openssh.com, aes128-ctr, aes192-ctr, aes256-ctr, arcfour256, arcfour128, aes128-cbc, 3des-cbc, blowfish-cbc, cast128-cbc, aes192-cbc, aes256-cbc, arcfour, rijndael-cbc@lysator.liu.se, aes128-gcm@openssh.com, aes256-gcm@openssh.com</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_enc_algo</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[chacha20-poly1305@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[aes128-ctr]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[aes192-ctr]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[aes256-ctr]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[arcfour256]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[arcfour128]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[aes128-cbc]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[3des-cbc]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[blowfish-cbc]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[cast128-cbc]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[aes192-cbc]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[aes256-cbc]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[arcfour]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[rijndael-cbc@lysator.liu.se]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[aes128-gcm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[aes256-gcm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssh_hsk</span> - Config SSH host key. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_hsk</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssh_hsk_algo</span> - Select one or more SSH hostkey algorithms. <span class="li-normal">type: list</span> <span class="li-normal">choices: ssh-rsa, ecdsa-sha2-nistp521, ecdsa-sha2-nistp384, ecdsa-sha2-nistp256, rsa-sha2-256, rsa-sha2-512, ssh-ed25519</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_hsk_algo</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ssh-rsa]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[ecdsa-sha2-nistp521]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[ecdsa-sha2-nistp384]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[ecdsa-sha2-nistp256]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[rsa-sha2-256]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[rsa-sha2-512]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[ssh-ed25519]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssh_hsk_override</span> - Enable/disable SSH host key override in SSH daemon. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_hsk_override</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssh_hsk_password</span> - Password for ssh-hostkey. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_hsk_password</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssh_kex_algo</span> - Select one or more SSH kex algorithms. <span class="li-normal">type: list</span> <span class="li-normal">choices: diffie-hellman-group1-sha1, diffie-hellman-group14-sha1, diffie-hellman-group14-sha256, diffie-hellman-group16-sha512, diffie-hellman-group18-sha512, diffie-hellman-group-exchange-sha1, diffie-hellman-group-exchange-sha256, curve25519-sha256@libssh.org, ecdh-sha2-nistp256, ecdh-sha2-nistp384, ecdh-sha2-nistp521</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_kex_algo</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[diffie-hellman-group1-sha1]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[diffie-hellman-group14-sha1]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[diffie-hellman-group14-sha256]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[diffie-hellman-group16-sha512]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[diffie-hellman-group18-sha512]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[diffie-hellman-group-exchange-sha1]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[diffie-hellman-group-exchange-sha256]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[curve25519-sha256@libssh.org]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[ecdh-sha2-nistp256]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[ecdh-sha2-nistp384]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[ecdh-sha2-nistp521]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssh_mac_algo</span> - Select one or more SSH MAC algorithms. <span class="li-normal">type: list</span> <span class="li-normal">choices: hmac-md5, hmac-md5-etm@openssh.com, hmac-md5-96, hmac-md5-96-etm@openssh.com, hmac-sha1, hmac-sha1-etm@openssh.com, hmac-sha2-256, hmac-sha2-256-etm@openssh.com, hmac-sha2-512, hmac-sha2-512-etm@openssh.com, hmac-ripemd160, hmac-ripemd160@openssh.com, hmac-ripemd160-etm@openssh.com, umac-64@openssh.com, umac-128@openssh.com, umac-64-etm@openssh.com, umac-128-etm@openssh.com</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_mac_algo</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[hmac-md5]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-md5-etm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-md5-96]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-md5-96-etm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-sha1]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-sha1-etm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-sha2-256]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-sha2-256-etm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-sha2-512]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-sha2-512-etm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-ripemd160]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-ripemd160@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[hmac-ripemd160-etm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[umac-64@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[umac-128@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[umac-64-etm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 <tr>
 <td>[umac-128-etm@openssh.com]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        </ul>
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure SSH config.
      fortinet.fortios.fortios_system_ssh_config:
          vdom: "{{ vdom }}"
          system_ssh_config:
              ssh_enc_algo: "chacha20-poly1305@openssh.com"
              ssh_hsk: "<your_own_value>"
              ssh_hsk_algo: "ssh-rsa"
              ssh_hsk_override: "disable"
              ssh_hsk_password: "<your_own_value>"
              ssh_kex_algo: "diffie-hellman-group1-sha1"
              ssh_mac_algo: "hmac-md5"


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
