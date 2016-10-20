
.. tag plugin_knife_windows_bootstrap_windows_ssh_options

This argument has the following options:

``--auth-timeout MINUTES``,
   The amount of time (in minutes) to wait for authentication to succeed. Default: ``2``.

``--bootstrap-no-proxy NO_PROXY_URL_or_IP``
   A URL or IP address that specifies a location that should not be proxied.

``--bootstrap-proxy PROXY_URL``
   The proxy server for the node that is the target of a bootstrap operation.

``--bootstrap-version VERSION``
   The version of the chef-client to install.

``-d DISTRO``, ``--distro DISTRO``
   .. tag knife_bootstrap_distro
   
   The template file to be used during a bootstrap operation. The following distributions are supported:
   
   * ``chef-full`` (the default bootstrap)
   * ``centos5-gems``
   * ``fedora13-gems``
   * ``ubuntu10.04-gems``
   * ``ubuntu10.04-apt``
   * ``ubuntu12.04-gems``
   * The name of a custom bootstrap template file.
   
   When this option is used, knife searches for the template file in the following order:
   
   #. The ``bootstrap/`` folder in the current working directory
   #. The ``bootstrap/`` folder in the chef-repo
   #. The ``bootstrap/`` folder in the ``~/.chef/`` directory
   #. A default bootstrap file.
   
   Do not use the ``--template-file`` option when ``--distro`` is specified.
   
   .. end_tag
   

``-G GATEWAY``, ``--ssh-gateway GATEWAY``
   The SSH tunnel or gateway that is used to run a bootstrap action on a machine that is not accessible from the workstation.

``-i IDENTITY_FILE``, ``--identity-file IDENTITY_FILE``
   The SSH identity file used for authentication. Key-based authentication is recommended.

``-j JSON_ATTRIBS``, ``--json-attributes JSON_ATTRIBS``
   A JSON string that is added to the first run of a chef-client.

``-N NAME``, ``--node-name NAME``
   The name of the node.

``--[no-]host-key-verify``
   Use ``--no-host-key-verify`` to disable host key verification. Default setting: ``--host-key-verify``.

``-p PORT``, ``--ssh-port PORT``
   The SSH port.

``-P PASSWORD``, ``--ssh-password PASSWORD``
   The SSH password. This can be used to pass the password directly on the command line. If this option is not specified (and a password is required) knife prompts for the password.

``--prerelease``
   Install pre-release gems.

``-r RUN_LIST``, ``--run-list RUN_LIST``
   A comma-separated list of roles and/or recipes to be applied.

``-s SECRET``, ``--secret``
   The encryption key that is used for values contained within a data bag item.

``--secret-file SECRET_FILE``
   The path to the file that contains the encryption key.

``--template-file TEMPLATE``
   The path to a template file to be used during a bootstrap operation.

``-x USER_NAME``, ``--ssh-user USER_NAME``
   The SSH user name.














.. end_tag

