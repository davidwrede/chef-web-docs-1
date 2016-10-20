
.. tag resource_service_notifies_enable_after_restart_or_reload

.. To enable a service after restarting or reloading it:

.. code-block:: ruby
 
   service 'apache' do
     supports :restart => true, :reload => true
     action :enable
   end

.. end_tag

