
.. tag windows_set_system_ruby

To set the system Ruby for the Microsoft Windows platform `the steps described for all platforms are true <https://docs.chef.io/install_dk.html#set-system-ruby>`_, but then require the following manual edits to the ``chef shell-init bash`` output for the Microsoft Windows platform:

#. Add quotes around the variable assignment strings.
#. Convert ``C:/`` to ``/c/``.
#. Save those changes.

.. end_tag

