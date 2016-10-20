
.. tag ctl_chef_backend_promote

Use the ``promote`` subcommand to promote the named node to be leader of the backend HA cluster. This command will:

* Complete with an exit code of ``0`` when the leader of the backend HA cluster is replaced as leader by the named node.
* Return an error message and a non-zero exit code if the named node is already leader because failover has been disabled (for either the cluster or the node) or if the new leader could not be promoted within the allowed time.

.. end_tag

