
.. tag resource_template_configure_file_from_local

.. To configure a file from a local template:

.. code-block:: ruby

   template '/tmp/config.conf' do
     local true
     source '/tmp/config.conf.erb'
   end

.. end_tag

