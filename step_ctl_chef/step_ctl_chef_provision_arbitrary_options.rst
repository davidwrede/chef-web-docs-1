
.. tag ctl_chef_provision_arbitrary_options

Use the ``--opt`` option to pass arbitrary command-line options. For example:

.. code-block:: bash

   $ chef provision (other options) --opt foo=bar

Use the ``--opt`` option more than once to pass more than one option. For example:

.. code-block:: bash

   $ chef provision (other options) --opt foo=bar --opt baz=qux

.. end_tag

