
.. tag resource_machine_file_syntax

The syntax for using the **machine_file** resource in a recipe is as follows:

.. code-block:: ruby

   machine_file 'name' do
     attribute 'value' # see properties section below
     ...
     action :action # see actions section below
   end

where 

* ``machine_file`` tells the chef-client to use the ``Chef::Provider::MachineFile`` provider during the chef-client run
* ``name`` is the name of the resource block; when the ``path`` property is not specified as part of a recipe, ``name`` is also the path to a file
* ``attribute`` is zero (or more) of the properties that are available for this resource
* ``:action`` identifies which steps the chef-client will take to bring the node into the desired state

.. end_tag

