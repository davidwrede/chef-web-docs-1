
.. tag policy_ctl_run_list

.. This file documents specifc behavior related to the -j option in the chef-client, chef-solo, and chef-shell executables.

Use this option to use policy files by specifying a JSON file that contains the following settings:

.. list-table::
   :widths: 200 300
   :header-rows: 1

   * - Setting
     - Description
   * - ``policy_group``
     - The name of a policy, as identified by the ``name`` setting in a Policyfile.rb file.
   * - ``policy_name``
     - The name of a policy group that exists on the Chef server.

For example:

.. code-block:: javascript

   {
     "policy_name": "appserver",
     "policy_group": "staging"
   }

.. end_tag

