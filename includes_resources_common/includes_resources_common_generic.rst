
.. tag resources_common_generic

A `resource <https://docs.chef.io/resource.html>`_ defines the desired state for a single configuration item present on a node that is under management by Chef. A resource collection---one (or more) individual resources---defines the desired state for the entire node. During a `chef-client run <https://docs.chef.io/chef_client.html#the-chef-client-title-run>`_, the current state of each resource is tested, after which the chef-client will take any steps that are necessary to repair the node and bring it back into the desired state.

.. end_tag

