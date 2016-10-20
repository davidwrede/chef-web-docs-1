
.. tag resource_machine_batch_stop_n_machines

.. To stop multiple machines in-parallel:

.. code-block:: ruby

   machine_batch do
     action :stop
     machines 'a', 'b', 'c', 'd', 'e'
   end

.. end_tag

