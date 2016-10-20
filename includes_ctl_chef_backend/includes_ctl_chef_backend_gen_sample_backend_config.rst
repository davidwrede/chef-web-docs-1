
.. tag ctl_chef_backend_gen_sample_backend_config

Use the ``gen-sample-backend-config`` subcommand to generate output that contains all of the backend HA cluster settings along with their default values. Use this subcommand to get the values for ``publish_address`` and ``vip_interface`` prior to bootstrapping a new node for the backend HA cluster.

.. warning:: Service-specific configuration settings---``etcd``, ``elasticsearch``, ``leaderl``, and ``postgresl``---are generated automatically by the backend and should only be tuned under guidance from Chef. Service-specific configuration settings must be identical on all nodes in the backend HA cluster unless directed otherwise.

.. end_tag

