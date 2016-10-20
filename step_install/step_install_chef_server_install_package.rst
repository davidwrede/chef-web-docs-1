
.. tag install_chef_server_install_package

.. This topic is hooked in globally to install topics for Chef server applications.


As a root user, install the Chef server package on the server, using the name of the package provided by Chef. For Red Hat and CentOS 6:

.. code-block:: bash

   $ rpm -Uvh /tmp/chef-server-core-<version>.rpm

For Ubuntu:

.. code-block:: bash

   $ dpkg -i /tmp/chef-server-core-<version>.deb

After a few minutes, the Chef server will be installed.

.. end_tag

