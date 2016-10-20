
.. tag config_rb_metadata_settings_gem

Specifies a gem dependency to be installed via the **chef_gem** resource after all cookbooks are synchronized, but before any other cookbook loading is done. Use this attribute once per gem dependency. For example:

.. code-block:: ruby

   gem "poise"
   gem "chef-sugar"
   gem "chef-provisioning"

.. end_tag

