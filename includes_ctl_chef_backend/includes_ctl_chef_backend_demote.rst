
.. tag ctl_chef_backend_demote

Use the ``demote`` subcommand to demote the current leader in the backend HA cluster, after which a new leader is elected from the group of available followers in the backend HA cluster. This command will:

* Complete with an exit code of ``0`` if the original leader was demoted and a new leader was elected successfully.
* Return an error message and a non-zero exit code if leader election is prevented because failover has been disabled (for either the cluster or the node) or if a new leader could not be elected within the allowed time.

.. end_tag

