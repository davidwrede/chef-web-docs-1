
.. tag resource_machine_batch_converge_n_machines

.. To converge multiple machines in-parallel:

.. code-block:: ruby

   machine_batch do
     action :converge
     machines 'a', 'b', 'c', 'd', 'e'
   end

.. end_tag

