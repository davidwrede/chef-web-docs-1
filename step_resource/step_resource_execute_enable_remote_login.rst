
.. tag resource_execute_enable_remote_login

.. To enable remote login on Mac OS X:

.. code-block:: ruby

   execute 'enable ssh' do 
     command '/usr/sbin/systemsetup -setremotelogin on'
     not_if '/usr/sbin/systemsetup -getremotelogin | /usr/bin/grep On'
     action :run
   end

.. end_tag

