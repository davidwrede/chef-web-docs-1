
.. tag resource_apt_package_install_package_using_local_file

.. To install a package using local file:

.. code-block:: ruby 

   apt_package 'jwhois' do    
     action :install
     source '/path/to/jwhois.deb'
   end   

.. end_tag

