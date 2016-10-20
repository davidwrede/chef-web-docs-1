
.. tag resource_machine_batch_syntax

The syntax for using the **machine_batch** resource in a recipe is as follows:

.. code-block:: ruby

   machine_batch 'name' do
     attribute 'value' # see properties section below
     ...
     action :action # see actions section below
   end

where 

* ``machine_batch`` tells the chef-client to use the ``Chef::Provider::MachineBatch`` provider during the chef-client run
* ``name`` is the name of the resource block
* ``attribute`` is zero (or more) of the properties that are available for this resource
* ``:action`` identifies which steps the chef-client will take to bring the node into the desired state

.. end_tag

