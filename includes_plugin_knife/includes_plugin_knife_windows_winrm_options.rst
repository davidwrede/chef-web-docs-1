
.. tag plugin_knife_windows_winrm_options

This argument has the following options:

``-a ATTR``, ``--attribute ATTR``
   The attribute used when opening an SSH connection. The default attribute is the FQDN of the host. Other possible values include a public IP address, a private IP address, or a hostname.

``-f CA_TRUST_FILE``, ``--ca-trust-file CA_TRUST_FILE``
   Optional. The certificate authority (CA) trust file used for SSL transport.

``-i IDENTITY_FILE``, ``--identity-file IDENTITY_FILE``
   The keytab file that contains the encryption key required by Kerberos-based authentication.

``--keytab-file KEYTAB_FILE``
   The keytab file that contains the encryption key required by Kerberos-based authentication.

``-m``, ``--manual-list``
   Define a search query as a space-separated list of servers.

``-p PORT``, ``--winrm-port PORT``
   The WinRM port. The TCP port on the remote system to which ``knife windows`` commands that are made using WinRM are sent. Default: ``5986`` when ``--winrm-transport`` is set to ``ssl``, otherwise ``5985``.

``-P PASSWORD``, ``--winrm-password PASSWORD``
   The WinRM password.

``-R KERBEROS_REALM``, ``--kerberos-realm KERBEROS_REALM``
   Optional. The administrative domain to which a user belongs.

``--returns CODES``
   A comma-delimited list of return codes that indicate the success or failure of the command that was run remotely.

``-S KERBEROS_SERVICE``, ``--kerberos-service KERBEROS_SERVICE``
   Optional. The service principal used during Kerberos-based authentication.

``SEARCH_QUERY``
   The search query used to return a list of servers to be accessed using SSH and the specified ``SSH_COMMAND``. This option uses the same syntax as the search subcommand.

``SSH_COMMAND``
   The command to be run against the results of a search query.

``--session-timeout MINUTES``
   The amount of time (in minutes) for the maximum length of a WinRM session.

``-t TRANSPORT``, ``--winrm-transport TRANSPORT``
   The WinRM transport type. Possible values: ``ssl`` or ``plaintext``.

``--winrm-authentication-protocol PROTOCOL``
   The authentication protocol to be used during WinRM communication. Possible values: ``basic``, ``kerberos`` or ``negotiate``. Default value: ``negotiate``.

``--winrm-ssl-verify-mode MODE``
   The peer verification mode that is used during WinRM communication. Possible values: ``verify_none`` or ``verify_peer``. Default value: ``verify_peer``.

``-x USERNAME``, ``--winrm-user USERNAME``
   The WinRM user name.

.. end_tag

