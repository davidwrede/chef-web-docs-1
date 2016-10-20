
.. tag delivery_config_json_setting_delivery_truck_lint_foodcritic_excludes

If the ``config.json`` file specifies:

.. code-block:: javascript

   "delivery-truck": {
     "lint": {
       "foodcritic": {
         "ignore_rules": ["RULE", "RULE", ...],
         "only_rules": ["RULE", "RULE", ...],
         "excludes": ["spec", "test"]
       }
     }
   }

then Foodcritic rules are not run against tests that are located in the specified directories, in this case the ``/spec`` and ``/test`` directories.

.. end_tag

