:source: fortios_system_saml.py

:orphan:

.. fortios_system_saml:

fortios_system_saml -- Global settings for SAML authentication in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and saml category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">system_saml</span> - Global settings for SAML authentication. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">cert</span> - Certificate to sign SAML messages. Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">default_login_page</span> - Choose default login page. <span class="li-normal">type: str</span> <span class="li-normal">choices: normal, sso</span></li>
        <li> <span class="li-head">default_profile</span> - Default profile for new SSO admin. Source system.accprofile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">entity_id</span> - SP entity ID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">idp_cert</span> - IDP certificate name. Source certificate.remote.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">idp_entity_id</span> - IDP entity ID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">idp_single_logout_url</span> - IDP single logout URL. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">idp_single_sign_on_url</span> - IDP single sign-on URL. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">life</span> - Length of the range of time when the assertion is valid (in minutes). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">portal_url</span> - SP portal URL. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">role</span> - SAML role. <span class="li-normal">type: str</span> <span class="li-normal">choices: identity-provider, service-provider</span></li>
        <li> <span class="li-head">server_address</span> - Server address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">service_providers</span> - Authorized service providers. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">assertion_attributes</span> - Customized SAML attributes to send along with assertion. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">type</span> - Type. <span class="li-normal">type: str</span> <span class="li-normal">choices: username, email, profile-name</span></li>
                </ul>
            <li> <span class="li-head">idp_entity_id</span> - IDP entity ID. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">idp_single_logout_url</span> - IDP single logout URL. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">idp_single_sign_on_url</span> - IDP single sign-on URL. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">prefix</span> - Prefix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sp_cert</span> - SP certificate name. Source certificate.remote.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sp_entity_id</span> - SP entity ID. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sp_portal_url</span> - SP portal URL. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sp_single_logout_url</span> - SP single logout URL. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sp_single_sign_on_url</span> - SP single sign-on URL. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">single_logout_url</span> - SP single logout URL. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">single_sign_on_url</span> - SP single sign-on URL. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable/disable SAML authentication . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tolerance</span> - Tolerance to the range of time when the assertion is valid (in minutes). <span class="li-normal">type: int</span></li>
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
      - name: Global settings for SAML authentication.
        fortios_system_saml:
          vdom:  "{{ vdom }}"
          system_saml:
            cert: "<your_own_value> (source certificate.local.name)"
            default_login_page: "normal"
            default_profile: "<your_own_value> (source system.accprofile.name)"
            entity_id: "<your_own_value>"
            idp_cert: "<your_own_value> (source certificate.remote.name)"
            idp_entity_id: "<your_own_value>"
            idp_single_logout_url: "<your_own_value>"
            idp_single_sign_on_url: "<your_own_value>"
            life: "11"
            portal_url: "<your_own_value>"
            role: "identity-provider"
            server_address: "<your_own_value>"
            service_providers:
             -
                assertion_attributes:
                 -
                    name: "default_name_17"
                    type: "username"
                idp_entity_id: "<your_own_value>"
                idp_single_logout_url: "<your_own_value>"
                idp_single_sign_on_url: "<your_own_value>"
                name: "default_name_22"
                prefix: "<your_own_value>"
                sp_cert: "<your_own_value> (source certificate.remote.name)"
                sp_entity_id: "<your_own_value>"
                sp_portal_url: "<your_own_value>"
                sp_single_logout_url: "<your_own_value>"
                sp_single_sign_on_url: "<your_own_value>"
            single_logout_url: "<your_own_value>"
            single_sign_on_url: "<your_own_value>"
            status: "enable"
            tolerance: "32"


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
