
.. tag ctl_chef_install

Use the ``chef install`` subcommand to evaluate a policy file and find a compatible set of cookbooks, build a run-list, cache it locally, and then emit a Policyfile.lock.json file that describes the locked policy set. The Policyfile.lock.json file may be used to install the locked policy set to other machines and may be pushed to a policy group on the Chef server to apply that policy to a group of nodes that are under management by Chef.

.. end_tag

