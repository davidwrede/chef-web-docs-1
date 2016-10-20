
.. tag resource_apt_package_install_without_recommends_suggests

.. To install without using recommend packages as a dependency:

.. code-block:: ruby 

   package 'apache2' do
     options '--no-install-recommends'
   end  

.. end_tag

