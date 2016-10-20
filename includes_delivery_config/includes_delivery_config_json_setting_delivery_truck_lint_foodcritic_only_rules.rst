
.. tag delivery_config_json_setting_delivery_truck_lint_foodcritic_only_rules

If the ``config.json`` file specifies:

.. code-block:: javascript

   "delivery-truck": {
     "lint": {
       "foodcritic": {
         "only_rules": ["FC002"],
         "excludes": ["DIRECTORY", "DIRECTORY", ...]
       }
     }
   }

then only the ``FC002`` Foodcritic rules is run.

.. end_tag

