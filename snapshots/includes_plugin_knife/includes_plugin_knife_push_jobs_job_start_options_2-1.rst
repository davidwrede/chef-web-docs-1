.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.


This argument has the following options:

``--timeout TIMEOUT``
   The maximum amount of time (in seconds) by which a job must complete, before it is stopped.

``-q QUORUM``, ``--quorum QUORUM``
   The minimum number of nodes that match the search criteria, are available, and acknowledge the job request. This can be expressed as a percentage (e.g. ``50%``) or as an absolute number of nodes (e.g. ``145``). Default value: ``100%``.

   For example, there are ten total nodes. If ``--quorum 80%`` is used and eight of those nodes acknowledge the job request, the command will be run against all of the available nodes. If two of the nodes were unavailable, the command would still be run against the remaining eight available nodes because quorum was met.

``-b``, ``--nowait``
   Exit immediately after starting a job instead of waiting for it to complete.

``--with-env ENVIRONMENT``
   Accept a JSON blob of environment variables and use those to set the variables for the client. For example ``'{"test": "foo"}'`` will set the push client environment variable "test" to "foo".

``--in-dir DIR``
   Execute the remote command in the directory ``DIR``.

``--file DATAFILE``
  Send the file to the client. Cleaned

``--capture``
  Capture stdin and stdout for this job.
