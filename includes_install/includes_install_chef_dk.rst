
.. tag install_chef_dk

To install the Chef development kit:

#. Visit this page: http://downloads.chef.io/chef-dk/. The Chef development kit supports Mac OS X, Red Hat Enterprise Linux, Ubuntu, and Microsoft Windows.
#. Select a platform, and then a package. (chef-docs uses the Mac OS X setup within the documentation.)
#. Click the download button.
#. Follow the steps in the installer and install the Chef development kit to your machine. The Chef development kit is installed to ``/opt/chefdk/`` on UNIX and Linux systems. 
#. When finished, open a command window and enter the following:

   .. code-block:: bash
   
      $ chef verify
   
   This will verify the main components of the Chef development kit: the chef-client, the Chef development kit library, and the tools that are built into the Chef development kit. The output should be similar to:
   
   .. code-block:: bash

      Running verification for component '...'
      ..........
      ---------------------------------------------
      Verification of component '...' succeeded.

#. Optional. Set the default shell. On Microsoft Windows it is strongly recommended to use Windows PowerShell and cmd.exe.

.. end_tag

