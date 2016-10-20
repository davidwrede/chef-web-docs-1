
.. tag windows_top_level_directory_names

Paths can be longer in UNIX and Linux environments than they can be in Microsoft Windows. Microsoft Windows will throw errors when path name lengths are too long. For this reason, it's often helpful to use a very short top-level directory in Microsoft Windows, much like what is done in UNIX and Linux. For example, Chef uses ``/opt/`` to install the Chef development kit on Mac OS X. A similar approach can be done on Microsoft Windows, by creating a top-level directory with a short name. For example: ``c:\chef``.

.. end_tag

