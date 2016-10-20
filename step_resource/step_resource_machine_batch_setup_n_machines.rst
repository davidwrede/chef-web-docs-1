
.. tag resource_machine_batch_setup_n_machines

.. To setup multiple machines in-parallel:

.. code-block:: ruby

   machine_batch do
     action :setup
     machines 'a', 'b', 'c', 'd', 'e'
   end

.. end_tag

