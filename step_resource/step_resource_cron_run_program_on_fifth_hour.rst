
.. tag resource_cron_run_program_on_fifth_hour

.. To run a program on the fifth hour of the day:

.. code-block:: ruby

   cron 'noop' do
     hour '5'
     minute '0'
     command '/bin/true'
   end

.. end_tag

