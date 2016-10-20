
.. tag install_chef_client_repo_manual_chef_directory

The .chef directory is used to store three files:

* knife.rb
* ORGANIZATION-validator.pem
* USER.pem

Where ``ORGANIZATION`` and ``USER`` represent strings that are unique to each organization. These files must be present in the .chef directory in order for a workstation to be able to connect to a Chef server.

To create the .chef directory:

#. In a command window, enter the following:

   .. code-block:: bash

      mkdir -p ~/chef-repo/.chef

#. After the .chef directory has been created, the following folder structure will be present on the local machine::

      chef-repo/
         .chef/        << the hidden directory
         certificates/
         config/
         cookbooks/
         data_bags
         environments/
         roles/

#. Add ``.chef`` to the ``.gitignore`` file to prevent uploading the contents of the ``.chef`` folder to GitHub. For example:

   .. code-block:: bash

      $ echo '.chef' >> ~/chef-repo/.gitignore

.. end_tag

