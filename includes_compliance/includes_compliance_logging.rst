
.. tag compliance_logging

The default directory where Chef Compliance is saving logs is: ``/var/log/chef-compliance/``. It contains a directory for each service, but you can follow all the logs with this command:

.. code-block:: ruby

   sudo chef-compliance-ctl tail

This command can also be run for an individual service by specifying the name of the service in the command. For example:

.. code-block:: bash

   sudo chef-compliance-ctl tail core

.. end_tag

