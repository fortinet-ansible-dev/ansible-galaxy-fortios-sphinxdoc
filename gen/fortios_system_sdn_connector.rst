:source: fortios_system_sdn_connector.py

:orphan:

.. _fortios_system_sdn_connector:

fortios_system_sdn_connector -- Configure connection to SDN Connector in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and sdn_connector category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">system_sdn_connector</span> - Configure connection to SDN Connector. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">access_key</span> - AWS access key ID. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">azure_region</span> - Azure server region. <span class="li-normal">type: str</span> <span class="li-normal">choices: global,  china,  germany,  usgov,  local</span></li>
            <li><span class="li-head">client_id</span> - Azure client ID (application ID). <span class="li-normal">type: str</span></li>
            <li><span class="li-head">client_secret</span> - Azure client secret (application key). <span class="li-normal">type: str</span></li>
            <li><span class="li-head">compartment_id</span> - Compartment ID. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">external_ip</span> - Configure GCP external IP. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - External IP name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">gcp_project</span> - GCP project name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">key_passwd</span> - Private key password. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">login_endpoint</span> - Azure Stack login enpoint. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">name</span> - SDN connector name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">nic</span> - Configure Azure network interface. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">ip</span> - Configure IP configuration. <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">name</span> - IP configuration name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
                            <li><span class="li-head">public_ip</span> - Public IP name. <span class="li-normal">type: str</span>
                            </ul>

                    <li><span class="li-head">name</span> - Network interface name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">oci_cert</span> - OCI certificate. Source certificate.local.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">oci_fingerprint</span> - OCI pubkey fingerprint. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">oci_region</span> - OCI server region. <span class="li-normal">type: str</span> <span class="li-normal">choices: phoenix,  ashburn,  frankfurt,  london</span></li>
            <li><span class="li-head">password</span> - Password of the remote SDN connector as login credentials. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">private_key</span> - Private key of GCP service account. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">region</span> - AWS region name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">resource_group</span> - Azure resource group. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">resource_url</span> - Azure Stack resource URL. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">route</span> - Configure GCP route. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Route name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">route_table</span> - Configure Azure route table. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Route table name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">route</span> - Configure Azure route. <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">name</span> - Route name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
                            <li><span class="li-head">next_hop</span> - Next hop address. <span class="li-normal">type: str</span>
                            </ul>

                    </ul>

            <li><span class="li-head">secret_key</span> - AWS secret access key. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">server</span> - Server address of the remote SDN connector. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">server_port</span> - Port number of the remote SDN connector. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">service_account</span> - GCP service account email. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">status</span> - Enable/disable connection to the remote SDN connector. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">subscription_id</span> - Azure subscription ID. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">tenant_id</span> - Tenant ID (directory ID). <span class="li-normal">type: str</span> <span class="li-normal">type:</span> Type of SDN connector. <span class="li-normal">type: str</span> <span class="li-normal">choices: aci,  aws,  azure,  gcp,  nsx,  nuage,  oci,  openstack</span></li>
            <li><span class="li-head">update_interval</span> - Dynamic object update interval (0 - 3600 sec, 0 means disabled). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">use_metadata_iam</span> - Enable/disable using IAM role from metadata to call API. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">user_id</span> - User ID. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">username</span> - Username of the remote SDN connector as login credentials. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">vpc_id</span> - AWS VPC ID. <span class="li-normal">type: str</span>
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
      - name: Configure connection to SDN Connector.
        fortios_system_sdn_connector:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          system_sdn_connector:
            access_key: "<your_own_value>"
            azure_region: "global"
            client_id: "<your_own_value>"
            client_secret: "<your_own_value>"
            compartment_id: "<your_own_value>"
            external_ip:
             -
                name: "default_name_9"
            gcp_project: "<your_own_value>"
            key_passwd: "<your_own_value>"
            login_endpoint: "<your_own_value>"
            name: "default_name_13"
            nic:
             -
                ip:
                 -
                    name: "default_name_16"
                    public_ip: "<your_own_value>"
                name: "default_name_18"
            oci_cert: "<your_own_value> (source certificate.local.name)"
            oci_fingerprint: "<your_own_value>"
            oci_region: "phoenix"
            password: "<your_own_value>"
            private_key: "<your_own_value>"
            region: "<your_own_value>"
            resource_group: "<your_own_value>"
            resource_url: "<your_own_value>"
            route:
             -
                name: "default_name_28"
            route_table:
             -
                name: "default_name_30"
                route:
                 -
                    name: "default_name_32"
                    next_hop: "<your_own_value>"
            secret_key: "<your_own_value>"
            server: "192.168.100.40"
            server_port: "36"
            service_account: "<your_own_value>"
            status: "disable"
            subscription_id: "<your_own_value>"
            tenant_id: "<your_own_value>"
            type: "aci"
            update_interval: "42"
            use_metadata_iam: "disable"
            user_id: "<your_own_value>"
            username: "<your_own_value>"
            vpc_id: "<your_own_value>"



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