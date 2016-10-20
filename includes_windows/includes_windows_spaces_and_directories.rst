
.. tag windows_spaces_and_directories

Directories that are used by Chef on the Microsoft Windows platform cannot have spaces. For example, ``/c/Users/Steven Danno`` will not work, but ``/c/Users/StevenDanno`` will.

A different issue exists with the knife command line tool that is also related to spaces and directories. The ``knife cookbook site install`` subcommand will fail when the Microsoft Windows directory contains a space.

.. end_tag

