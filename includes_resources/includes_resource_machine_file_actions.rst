
.. tag resource_machine_file_actions

This resource has the following actions:

``:delete``
   Use to delete a file from a machine.

``:download``
   Use to download a file from a machine.

``:nothing``
   .. tag resources_common_actions_nothing
   
   Define this resource block to do nothing until notified by another resource to take action. When this resource is notified, this resource block is either run immediately or it is queued up to be run at the end of the chef-client run.
   
   .. end_tag
   

``:upload``
   Default. Use to upload a file to a machine.

.. end_tag

