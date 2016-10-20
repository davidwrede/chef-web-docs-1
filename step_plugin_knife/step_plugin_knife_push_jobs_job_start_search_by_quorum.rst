
.. tag plugin_knife_push_jobs_job_start_search_by_quorum

To search for nodes assigned the role ``webapp``, and where 90% of those nodes must be available, run the following command:

.. code-block:: bash

   $ knife job start --quorum 90% 'chef-client' --search 'role:webapp'


.. end_tag

