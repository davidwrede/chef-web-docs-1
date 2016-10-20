
.. tag ruby_set_system_ruby_as_chefdk_ruby_windows

You can use ``chef shell-init`` with Windows PowerShell.

To try it in your current session:

.. code-block:: bash

   chef shell-init powershell | Invoke-Expression

To enable it permanently:

.. code-block:: bash

   "chef shell-init powershell | Invoke-Expression" >> $PROFILE

.. end_tag

