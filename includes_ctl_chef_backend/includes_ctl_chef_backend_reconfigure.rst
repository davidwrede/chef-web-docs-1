
.. tag ctl_chef_backend_reconfigure

Use the ``reconfigure`` subcommand to reconfigure a machine in the Chef server backend HA cluster. This subcommand will also restart any services for which the ``service_name['enabled']`` setting is set to ``true``.

This subcommand has the following syntax:

.. code-block:: bash

   $ chef-backend-ctl reconfigure

.. end_tag

