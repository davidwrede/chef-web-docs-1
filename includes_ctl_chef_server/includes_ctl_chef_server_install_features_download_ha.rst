
.. tag ctl_chef_server_install_features_download_ha

The ``install`` subcommand downloads packages from https://packages.chef.io/ by default. For systems that are not behind a firewall (and have connectivity to https://packages.chef.io/), the Chef management console package can be installed as described below:

Chef Manage
   Use Chef management console to manage data bags, attributes, run-lists, roles, environments, and cookbooks from a web user interface.

   On each front end server in the Chef server configuration, run:

   .. code-block:: bash

      $ chef-server-ctl install chef-manage

   then:

   .. code-block:: bash

      $ chef-server-ctl reconfigure

   and then:

   .. code-block:: bash

      $ chef-manage-ctl reconfigure

   This updates the Chef server and creates the ``/etc/opscode-manage/secrets.rb`` file. When running the Chef management console 1.11 (or higher), copy the ``secrets.rb`` file in the ``/etc/opscode-manage`` directory on one of the frontend servers to the same directory on each of the other frontend servers, and then rerun ``chef-manage-ctl reconfigure`` so the copied ``/etc/opscode-manage/secrets.rb`` file gets used correctly.

   .. note:: .. tag chef_license_reconfigure_manage
             
             Starting with the Chef management console 2.3.0, the `Chef MLSA <https://docs.chef.io/chef_license.html>`__ must be accepted when reconfiguring the product. If the Chef MLSA has not already been accepted, the reconfigure process will prompt for a ``yes`` to accept it. Or run ``chef-manage-ctl reconfigure --accept-license`` to automatically accept the license.
             
             .. end_tag
             




.. end_tag

