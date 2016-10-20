
.. tag plugin_knife_windows_bootstrap_ssh

To bootstrap a Microsoft Windows machine using SSH:

.. code-block:: bash

   $ knife bootstrap windows ssh ec2-50-xx-xx-124.compute-1.amazonaws.com -r 'role[webserver],role[production]' -x Administrator -i ~/.ssh/id_rsa

.. end_tag

