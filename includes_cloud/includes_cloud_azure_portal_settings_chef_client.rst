
.. tag cloud_azure_portal_settings_chef_client

Before virtual machines are created using the Azure portal, some chef-client-specific settings will need to be identified so they may be provided to the Azure portal during the virtual machine creation workflow. These settings are available from the chef-client configuration settings:

#. The ``chef_server_url`` and ``validaton_client_name``. These are settings in the `client.rb file <https://docs.chef.io/config_rb_client.html>`_.

#. The file for the `validator key <https://docs.chef.io/chef_private_keys.html>`_.

.. end_tag

