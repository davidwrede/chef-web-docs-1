
.. tag resource_machine_batch_destroy_n_machines

.. To delete multiple machines in-parallel:

.. code-block:: ruby

   machine_batch do
     action :delete
     machines 'a', 'b', 'c', 'd', 'e'
   end

.. end_tag

