
.. tag config_rb_metadata_settings_example_ohai_version

For example, to match any 8.x version of Ohai, but not 7.x or 9.x:

.. code-block:: ruby

   ohai_version "~> 8"

Or matches any 8.x (or higher) version of Ohai:

.. code-block:: ruby

   ohai_version ">= 8"

.. end_tag

