
.. tag resource_machines_use_a_loop_to_create_many_machines

.. To create multiple machines using a loop:

.. code-block:: ruby

   1.upto(10) do |i|
     machine "hadoop#{i}" do
       recipe 'hadoop'
     end
   end

.. end_tag

