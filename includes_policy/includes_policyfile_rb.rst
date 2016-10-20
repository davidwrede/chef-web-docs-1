
.. tag policyfile_rb

A Policyfile file allows you to specify in a single document the cookbook revisions and recipes that should be applied by the chef-client. A Policyfile file is uploaded to the Chef server, where it is associated with a group of nodes. When these nodes are configured by the chef-client, the chef-client will make decisions based on settings in the policy file, and will build a run-list based on that information. A Policyfile file may be versioned, and then promoted through deployment stages to safely and reliably deploy new configuration. 

.. end_tag

