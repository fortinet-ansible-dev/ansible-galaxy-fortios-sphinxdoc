
Run Your First Playbook
==============================

This document explains how to run your first FortiOS Ansible playbook.

--------------

With FortiOS Galaxy collection, you are always recommended to run
FortiOS module in ``httpapi`` manner. The first step is to prepare your
host inventory with which you can use ``ansible-vault`` to encrypt or
decrypt your secrets for the sake of confidentiality.

Prepare host inventory
~~~~~~~~~~~~~~~~~~~~~~

in our case we create a file named ``hosts``:

::

   [fortigates]
   fortigate01 ansible_host=192.168.190.130

   [fortigates:vars]
   ansible_network_os=fortinet.fortios.fortios
   ansible_log_path=/tmp/ansible.network.log
   ansible_user=admin
   ansible_password=YOUR_OWN_VALUE
   ansible_httpapi_session_key={"access_token":"YOUR_OWN_VALUE"}

FortiOS supports two ways to authenticate Ansible: ``ansible_user`` and ``ansible_password`` pair based; ``ansible_httpapi_session_key`` access token based. The access token method is preferred as it offers enhanced security by avoiding password exposure and ensures that requests originate from the intended source.

``fortios_access_token`` is a way for authentication, and it will be deprecated in the future, please use ``ansible_httpapi_session_key`` instead.


for how to generate an API token, visit page `FortiOS API Spec`_.


Write the playbook
~~~~~~~~~~~~~~~~~~

in the example: ``test.yml`` is going to modify the FortiGate
device's hostname, please modify the variable values if needed.

::

   - hosts: fortigate01
     connection: httpapi
     collections:
     - fortinet.fortios
     vars:
      vdom: "root"
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
      ansible_httpapi_port: 443
     tasks:
      - name: Configure global attributes.
        fortios_system_global:
           vdom:  "{{ vdom }}"
           system_global:
               hostname: 'CustomHostName'

there are several options which might need you special care:

-  **connection** : ``httpapi`` is preferred.
-  **collections** : The namespace must be ``fortinet.fortios``
-  **ansible_httpapi_use_ssl** and **ansible_httpapi_port**: by
   default when your fortiOS device is licensed, the https is enabled.
   there is one exception: uploading vmlicence to a newly installed FOS instance, where you should set
   ``ansible_httpapi_use_ssl: no`` and ``ansible_httpapi_port: 80``. Please see `Import licence to FOS`_ for more details.

Run the playbook
~~~~~~~~~~~~~~~~

::

   ansible-playbook -i hosts test.yml

you can also observe the verbose output by adding option at the tail:
``-vvv``.

.. _Import licence to FOS: faq.html#how-to-import-a-license
.. _FortiOS API Spec: https://fndn.fortinet.net/index.php?/fortiapi/1-fortios/92/
