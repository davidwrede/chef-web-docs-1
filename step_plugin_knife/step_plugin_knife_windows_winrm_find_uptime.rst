
.. tag plugin_knife_windows_winrm_find_uptime

To find the uptime of all web servers, enter:

.. code-block:: bash

   $ knife winrm "role:web" "net stats srv" -x Administrator -P password

.. end_tag

