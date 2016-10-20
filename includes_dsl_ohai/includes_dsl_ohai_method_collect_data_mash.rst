
.. tag dsl_ohai_method_collect_data_mash

Use a mash to store data. This is done by creating a new mash, and then setting an attribute to it. For example:

.. code-block:: ruby

   provides 'name_of_mash'
   name_of_mash Mash.new
   name_of_mash[:attribute] = 'value'

.. end_tag

