
.. tag ohai_custom_plugin_logs_rescue

Use the ``rescue`` clause to make sure that a log message is always provided. For example:

.. code-block:: ruby

   rescue LoadError => e
     Ohai::Log.debug('ip_scopes: cannot load gem, plugin disabled: #{e}')
   end

.. end_tag

