
.. tag ohai_custom_plugin_example_use_mixin_library

The following Ohai example shows a plugin can use a ``mixin`` library and also depend on another plugin:

.. code-block:: ruby

   require 'ohai/mixin/os'
   
   Ohai.plugin(:Os) do
     provides 'os', 'os_version'
     depends 'kernel'
   
     collect_data do
       os collect_os
       os_version kernel[:release]
     end
   end

.. end_tag

