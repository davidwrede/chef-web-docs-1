
.. tag resource_cron_run_entry_when_folder_exists

.. To run an entry if a folder exists:

.. code-block:: ruby

   cron 'ganglia_tomcat_thread_max' do
     command "/usr/bin/gmetric 
       -n 'tomcat threads max' 
       -t uint32 
       -v '/usr/local/bin/tomcat-stat 
       --thread-max'"
     only_if do File.exist?('/home/jboss') end
   end

.. end_tag

