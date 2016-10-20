
.. tag resource_machine_image_add_apache_to_image

.. To add Apache to a machine image, and then build a machine:

.. code-block:: ruby

   machine_image 'web_image' do
     recipe 'apache2'
   end
   
   machine 'web_machine' do
    from_image 'web_image'
   end

.. end_tag

