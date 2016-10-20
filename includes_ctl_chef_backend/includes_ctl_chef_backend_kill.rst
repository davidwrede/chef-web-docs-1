
.. tag ctl_chef_backend_kill

Use the ``kill`` subcommand to send a ``SIGKILL`` to all services on a machine in the Chef server backend HA cluster. This command can also be run for an individual service by specifying the name of the service in the command. 

This subcommand has the following syntax:

.. code-block:: bash

   $ chef-backend-ctl kill SERVICE_NAME

where ``SERVICE_NAME`` represents the name of any service that is listed after running the ``service-list`` subcommand.

.. end_tag

