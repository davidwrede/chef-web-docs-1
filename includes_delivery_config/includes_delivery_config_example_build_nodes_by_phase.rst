
.. tag delivery_config_example_build_nodes_by_phase

The following example shows how to specify build nodes to be used for specific phases.

.. code-block:: javascript

   "build_nodes": {
     "provision": ["name:builder-*-2.delivery.chef.co AND platform_version:14.04"],
     "deploy": ["name:builder-*-2.delivery.chef.co AND platform_version:14.04"],
     "functional": ["name:builder* AND platform_version:14.04 NOT name:builder-*-2.delivery.chef.co"]
   }

.. end_tag

