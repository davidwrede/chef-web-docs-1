
.. tag resource_apt_update_at_start_of_client_run

.. To update the Apt repository at the start of a chef-client run:

.. code-block:: ruby

   apt_update if node['platform_family'] == 'debian' do
     action :update
   end 

.. end_tag

