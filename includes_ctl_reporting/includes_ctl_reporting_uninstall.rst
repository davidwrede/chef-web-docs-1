
.. tag ctl_reporting_uninstall

The ``uninstall`` subcommand is used to remove the Reporting add-on to the Chef server, but without removing any of the data. This subcommand will shut down all services (including the ``runit`` process supervisor).

This subcommand has the following syntax:

.. code-block:: bash

   $ opscode-reporting-ctl uninstall

.. note:: To revert the ``uninstall`` subcommand, run the ``reconfigure`` subcommand (because the ``start`` subcommand is disabled by the ``uninstall`` command). 

.. end_tag

