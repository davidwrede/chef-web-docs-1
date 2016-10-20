
.. tag ctl_chef_backend_int

Use the ``int`` subcommand to send a ``SIGINT`` to all services on a machine in the Chef server backend HA cluster. This command can also be run for an individual service by specifying the name of the service in the command. 

This subcommand has the following syntax:

.. code-block:: bash

   $ chef-backend-ctl int SERVICE_NAME

where ``SERVICE_NAME`` represents the name of any service that is listed after running the ``service-list`` subcommand.

.. end_tag

