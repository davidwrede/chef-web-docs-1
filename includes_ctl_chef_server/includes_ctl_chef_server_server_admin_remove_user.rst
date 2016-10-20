
.. tag ctl_chef_server_server_admin_remove_user

The ``remove-server-admin-permissions`` subcommand is used to remove a user from the ``server-admins`` group. Run the command once per user removed.

This subcommand has the following syntax:

.. code-block:: bash

   $ chef-server-ctl remove-server-admin-permissions USER_NAME

where ``USER_NAME`` is the user to remove from the list of server administrators.

For example:

.. code-block:: bash

   $ chef-server-ctl remove-server-admin-permissions bob

returns:

.. code-block:: bash

   User bob was removed from server-admins. This user can no longer
   list, read, and create users for this Chef Server except for where
   they have default permissions (such as within an org).

.. end_tag

