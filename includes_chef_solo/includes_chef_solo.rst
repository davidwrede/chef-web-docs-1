
.. tag chef_solo_summary

chef-solo is an open source version of the chef-client that allows using cookbooks with nodes without requiring access to a Chef server. chef-solo uses `Chef local mode <https://docs.chef.io/ctl_chef_client.html#run-in-local-mode>`_, and **does not support** the following:

* Centralized distribution of cookbooks
* A centralized API that interacts with and integrates infrastructure components
* Authentication or authorization

.. note:: chef-solo can be run as a daemon. 


.. end_tag

