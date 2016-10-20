
.. tag ctl_chef_backend_gen_server_config

Use the ``gen-server-config`` subcommand to generate output for the ``chef-server.rb`` configuration file. This command may be run from any machine in the backend HA cluster, but must be run separately for each node that is part of the frontend group. This command will:

* Complete with an exit code of ``0`` if the ``chef-server.rb`` file is created successfully.
* Return an error message and a non-zero exit code if a node has  not been bootstrapped or joined or if a FQDN is not provided.

.. end_tag

