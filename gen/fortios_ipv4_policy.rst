:source: fortios_ipv4_policy.py

:orphan:

.. _fortios_ipv4_policy:

fortios_ipv4_policy -- Manage IPv4 policy objects on Fortinet FortiOS firewall devices
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.3

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module provides management of firewall IPv4 policies on FortiOS devices.


Requirements
------------
The below requirements are needed on the host that executes this module.

- pyFG


Parameters
----------

.. raw:: html

    <ul>

    <li><span class="li-head">id</span> - "Policy ID. Warning: policy ID number is different than Policy sequence number. The policy ID is the number assigned at policy creation. The sequence number represents the order in which the Fortigate will evaluate the rule for policy enforcement, and also the order in which rules are listed in the GUI and CLI. These two numbers do not necessarily correlate: this module is based off policy ID. TIP: policy ID can be viewed in the GUI by adding 'ID' to the display columns" <span class="li-required">required</span></li>
    <li><span class="li-head">state</span> - Specifies if policy I(id) need to be added or deleted. <span class="li-normal">choices: ['present', 'absent'] <span class="li-normal">default: present</span></li>
    <li><span class="li-head">src_intf</span> - Specifies source interface name(s). <span class="li-normal">default: any</span></li>
    <li><span class="li-head">dst_intf</span> - Specifies destination interface name(s). <span class="li-normal">default: any</span></li>
    <li><span class="li-head">src_addr</span> - Specifies source address (or group) object name(s). Required when I(state=present).</li>
    <li><span class="li-head">src_addr_negate</span> - Negate source address param. <span class="li-normal">default: false</span> <span class="li-normal">type: bool</span></li>
    <li><span class="li-head">dst_addr</span> - Specifies destination address (or group) object name(s). Required when I(state=present).</li>
    <li><span class="li-head">dst_addr_negate</span> - Negate destination address param. <span class="li-normal">default: false</span> <span class="li-normal">type: bool</span></li>
    <li><span class="li-head">policy_action</span> - Specifies accept or deny action policy. Required when I(state=present). <span class="li-normal">choices: ['accept', 'deny']</li>
    <li><span class="li-head">service</span> - "Specifies policy service(s), could be a list (ex: ['MAIL','DNS']). Required when I(state=present)."</li>
    <li><span class="li-head">aliases</span> -</li>
    <li><span class="li-head">service_negate</span> - Negate policy service(s) defined in service value. <span class="li-normal">default: false</span> <span class="li-normal">type: bool</span></li>
    <li><span class="li-head">schedule</span> - defines policy schedule. <span class="li-normal">default: 'always'</span></li>
    <li><span class="li-head">nat</span> - Enable or disable Nat. <span class="li-normal">default: false</span> <span class="li-normal">type: bool</span></li>
    <li><span class="li-head">fixedport</span> - Use fixed port for nat. <span class="li-normal">default: false</span> <span class="li-normal">type: bool</span></li>
    <li><span class="li-head">poolname</span> - Specifies NAT pool name.</li>
    <li><span class="li-head">av_profile</span> - Specifies Antivirus profile name.</li>
    <li><span class="li-head">webfilter_profile</span> - Specifies Webfilter profile name.</li>
    <li><span class="li-head">ips_sensor</span> - Specifies IPS Sensor profile name.</li>
    <li><span class="li-head">application_list</span> - Specifies Application Control name.</li>
    <li><span class="li-head">logtraffic</span> -</li>
    <li><span class="li-head">description</span> -</li>
    <li><span class="li-head">logtraffic_start</span> -</li>
    <li><span class="li-head">description</span> -</li>
    <li><span class="li-head">comment</span> - free text to describe policy.
    </ul>




Notes
-----

.. note::


   - Requires fortiosapi library developed by Fortinet

   - Run as a local_action in your playbook



Examples
--------

.. code-block:: yaml+jinja

    


Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">firewall_address_config</span> - full firewall addresses config string <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span></li>
    <li><span class="li-return">change_string</span> - The commands executed by the module <span class="li-normal">returned: only if config changed</span> <span class="li-normal">type: str</span></li>
    <li><span class="li-return">msg_error_list</span> - "List of errors returned by CLI (use -vvv for better readability)." <span class="li-normal">returned: only when error</span> <span class="li-normal">type: str</span></li>
    </ul>



Status
------

- This module is not guaranteed to have a backwards compatible interface.



Authors
-------

- Benjamin Jolivot (@bjolivot)



.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.