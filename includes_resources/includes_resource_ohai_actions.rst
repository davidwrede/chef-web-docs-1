
.. tag resource_ohai_actions

This resource has the following actions:

``:nothing``
   .. tag resources_common_actions_nothing
   
   Define this resource block to do nothing until notified by another resource to take action. When this resource is notified, this resource block is either run immediately or it is queued up to be run at the end of the chef-client run.
   
   .. end_tag
   

``:reload``
   Default. Reload the Ohai configuration on a node.

.. end_tag

