
.. tag ctl_chef_provision_syntax

This subcommand has the following syntax:

To create machines that operate using only a local Policyfile.rb:

.. code-block:: bash

   $ chef provision POLICY_GROUP --policy-name POLICY_NAME (options)

To create machines that operate using a Policyfile.rb that is synchronized with the Chef server before each chef-client run:

.. code-block:: bash

   $ chef provision POLICY_GROUP --sync PATH (options)

To create machines that will not use a Policyfile.rb file:

.. code-block:: bash

   $ chef provision --no-policy (options)

.. end_tag

