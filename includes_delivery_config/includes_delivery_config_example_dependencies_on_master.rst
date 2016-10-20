
.. tag delivery_config_example_dependencies_on_master

The following example shows a run-time dependency against the master branch of a project named ``BackendAPI``:

.. code-block:: javascript

   {
     "version": "2",
     "build_cookbook": {
       "name": "build-cookbook",
       "path": ".delivery/build-cookbook"
     },
     "skip_phases": [],
     "dependencies": ["BackendAPI"]
   }


.. end_tag

