
.. tag plugin_knife_windows_winrm_requirements

This subcommand requires WinRM to be installed, and then configured correctly, including ensuring the correct ports are open. For more information, see: http://msdn.microsoft.com/en-us/library/aa384372(v=vs.85).aspx and/or http://support.microsoft.com/kb/968930. Use the quick configuration option in WinRM to allow outside connections and the entire network path from knife (and the workstation):

.. code-block:: bash

   $ winrm quickconfig -q

The following WinRM configuration settings should be updated:

.. list-table::
   :widths: 200 300
   :header-rows: 1

   * - Setting
     - Description
   * - ``MaxMemoryPerShellMB``
     - The chef-client and Ohai typically require more memory than the default setting allows. Increase this value to ``300MB``. Only required on Windows Server 2008 R2 Standard and older. The default in Windows Server 2012 was increased to ``1024MB``.
   * - ``MaxTimeoutms``
     - A bootstrap command can take longer than allowed by the default setting. Increase this value to ``1800000`` (30 minutes).
   * - ``AllowUnencrypted``
     - Set this value to ``true`` for development and testing purposes.
   * - ``Basic``
     - Set this value to ``true`` for development and testing purposes. The ``knife windows`` subcommand supports Kerberos and Basic authentication schemes.

To update these settings, run the following commands:

.. code-block:: bash

   $ winrm set winrm/config/winrs '@{MaxMemoryPerShellMB="300"}'

and:

.. code-block:: bash

   $ winrm set winrm/config '@{MaxTimeoutms="1800000"}'

and:

.. code-block:: bash

   $ winrm set winrm/config/service '@{AllowUnencrypted="true"}'

and then:

.. code-block:: bash

   $ winrm set winrm/config/service/auth '@{Basic="true"}'

Ensure that the Windows Firewall is configured to allow WinRM connections between the workstation and the Chef server. For example:

.. code-block:: bash

   $ netsh advfirewall firewall set rule name="Windows Remote Management (HTTP-In)" profile=public protocol=tcp localport=5985 remoteip=localsubnet new remoteip=any

.. end_tag

