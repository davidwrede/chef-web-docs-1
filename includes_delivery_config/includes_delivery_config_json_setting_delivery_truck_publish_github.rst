
.. tag delivery_config_json_setting_delivery_truck_publish_github

If the ``config.json`` file specifies the following cookbooks are published to a GitHub repository:

.. code-block:: javascript

   "delivery-truck":{
     "publish": {
       "github": "chef/chef-web-docs"
     }
   }

where ``"chef/chef-web-docs"`` represents the organization/repository to which the ``build-cookbook`` belongs.

This publishing option requires the ``github`` deploy key for that repository to be available from a data bag on the Chef server that is part of this Chef Automate configuration.

.. end_tag

