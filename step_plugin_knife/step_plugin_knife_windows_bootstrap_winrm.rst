
.. tag plugin_knife_windows_bootstrap_winrm

To bootstrap a Microsoft Windows machine using WinRM:

.. code-block:: bash

   $ knife bootstrap windows winrm ec2-50-xx-xx-124.compute-1.amazonaws.com -r 'role[webserver],role[production]' -x Administrator -P 'super_secret_password'

.. end_tag

