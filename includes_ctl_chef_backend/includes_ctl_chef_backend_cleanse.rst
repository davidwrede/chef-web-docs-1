
.. tag ctl_chef_backend_cleanse

The ``cleanse`` subcommand is used to re-set a machine in the Chef server backend HA cluster to the state it was in prior to the first time the ``reconfigure`` subcommand is run. This command will destroy all data, configuration files, and logs. The software that was put on-disk by the package installation will remain; re-run ``chef-backend-ctl reconfigure`` to recreate the default data and configuration files.

.. end_tag

