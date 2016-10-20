
.. tag ctl_chef_backend_gen_server_config_steps

#. On any node in the backend HA cluster, run the following command for each node in the frontend group:

   .. code-block:: bash

      $ chef-backend-ctl gen-server-config FQDN -f chef-server.rb.fqdn

   where ``FQDN`` is the FQDN for the frontend machine. The generated ``chef-server.rb`` file will contain all of the values necessary for any frontend Chef server to connect to and bootstrap against the backend HA cluster.

#. On each frontend machine, install the ``chef-server-core`` package (version 12.4.0 or higher).
#. On each frontend machine, copy the generated ``chef-server.rb``.fqdn to ``/etc/opscode/chef-server.rb``.
#. On each frontend machine, with root permission, run the following command:

   .. code-block:: bash

      $ chef-server-ctl reconfigure

.. end_tag

