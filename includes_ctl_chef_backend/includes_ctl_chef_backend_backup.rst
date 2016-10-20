
.. tag ctl_chef_backend_backup

Use the ``backup`` subcommand is to backup the data for a node in the backend HA cluster. This command is typically run against a follower node. Use the ``--force`` option to run this command against all nodes in the backend HA cluster. The backup is created as a tar.gz file and is located in ``/var/opt/chef-backup/``.

.. end_tag

