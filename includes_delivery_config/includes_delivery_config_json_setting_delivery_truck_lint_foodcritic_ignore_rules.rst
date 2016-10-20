
.. tag delivery_config_json_setting_delivery_truck_lint_foodcritic_ignore_rules

If the ``config.json`` file specifies:

.. code-block:: javascript

   "delivery-truck": {
     "lint": {
       "foodcritic": {
         "ignore_rules": ["FC009", "FC057", "FC058"],
         "excludes": ["DIRECTORY", "DIRECTORY", ...]
       }
     }
   }

then all Foodcritic rules except ``FC009``, ``FC057``, and ``FC058``  rules are run.

.. end_tag

