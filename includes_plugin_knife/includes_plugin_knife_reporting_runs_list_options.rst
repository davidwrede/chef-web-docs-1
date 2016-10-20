
.. tag plugin_knife_reporting_runs_list_options

This argument has the following options:

``-e MM-DD-YYYY``, ``--endtime MM-DD-YYYY``
   Find runs with an end time less than or equal to the specified date. This option must be used in conjunction with ``--starttime`` and may define up to a 90-day time period.

``RUN_ID``
   Required. The identifier for a chef-client run.

``-r N``, ``--rows N``
   The number of rows to be returned.

``-s MM-DD-YYYY``, ``--starttime MM-DD-YYYY``
   Find runs with a start time greater than or equal to the specified date. This option must be used in conjunction with ``--endtime`` and may define up to a 90-day time period.

``-u``, ``--unixtimestamps``
   Show start and end times as UNIX timestamps. This option may be used when the ``--endtime`` and ``--starttime`` options are used.

.. end_tag

