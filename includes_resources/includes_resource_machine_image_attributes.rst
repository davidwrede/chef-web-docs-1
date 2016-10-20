
.. tag resource_machine_image_attributes

This resource has the following properties:
   
``attributes``
   Use to specify a hash of attributes to be applied to the machine image.
   
``chef_environment``
   The name of the environment.
   
``complete``
   Use to specify if all of the attributes specified in ``attributes`` represent a complete specification for the machine image. When true, any attributes not specified in ``attributes`` will be reset to their default values.
   
``ignore_failure``
   **Ruby Types:** TrueClass, FalseClass

   Continue running a recipe if a resource fails for any reason. Default value: ``false``.
   
``image_options``
   **Ruby Type:** Hash

   Use to specify options that are used with this machine image.
   
``name``
   The name of the machine image.
   
``notifies``
   **Ruby Type:** Symbol, 'Chef::Resource[String]'

   .. tag resources_common_notification_notifies
   
   A resource may notify another resource to take action when its state changes. Specify a ``'resource[name]'``, the ``:action`` that resource should take, and then the ``:timer`` for that action. A resource may notifiy more than one resource; use a ``notifies`` statement for each resource to be notified.
   
   .. end_tag
   

   .. tag resources_common_notification_timers
   
   A timer specifies the point during the chef-client run at which a notification is run. The following timers are available:
   
   ``:before``
      Specifies that the action on a notified resource should be run before processing the resource block in which the notification is located. 
   
   ``:delayed``
      Default. Specifies that a notification should be queued up, and then executed at the very end of the chef-client run.
   
   ``:immediate``, ``:immediately``
      Specifies that a notification should be run immediately, per resource notified.
   
   .. end_tag
   

   .. tag resources_common_notification_notifies_syntax
   
   The syntax for ``notifies`` is:
   
   .. code-block:: ruby
   
      notifies :action, 'resource[name]', :timer
   
   .. end_tag
   
   
``raw_json``
   The machine image as JSON data. For example:
       
   .. code-block:: javascript
       
      {
       
      }
   
``recipe``
   Use to add a recipe to the run-list for the machine image. Each ``recipe`` adds a single recipe to the run-list. The order in which ``recipe`` defines the run-list is the order in which Chef will execute the run-list on the machine image.
   
``remove_recipe``
   Use to remove a recipe from the run-list for the machine image.
   
``remove_role``
   Use to remove a role from the run-list for the machine image.
   
``retries``
   **Ruby Type:** Integer

   The number of times to catch exceptions and retry the resource. Default value: ``0``.
   
``retry_delay``
   **Ruby Type:** Integer

   The retry delay (in seconds). Default value: ``2``.
   
``role``
   Use to add a role to the run-list for the machine image.
   
``run_list``
   Use to specify the run-list to be applied to the machine image.
	   
   .. tag node_run_list
   
   A run-list defines all of the information necessary for Chef to configure a node into the desired state. A run-list is:
   
   * An ordered list of roles and/or recipes that are run in the exact order defined in the run-list; if a recipe appears more than once in the run-list, the chef-client will not run it twice
   * Always specific to the node on which it runs; nodes may have a run-list that is identical to the run-list used by other nodes
   * Stored as part of the node object on the Chef server
   * Maintained using knife, and then uploaded from the workstation to the Chef server, or is maintained using the Chef management console
   
   .. end_tag
   
       
   .. tag node_run_list_format
   
   A run-list must be in one of the following formats: fully qualified, cookbook, or default. Both roles and recipes must be in quotes, for example:
   
   .. code-block:: ruby
   
      'role[NAME]'
   
   or 
   
   .. code-block:: ruby
   
      'recipe[COOKBOOK::RECIPE]'
   
   Use a comma to separate roles and recipes when adding more than one item the run-list: 
   
   .. code-block:: ruby
   
      'recipe[COOKBOOK::RECIPE],COOKBOOK::RECIPE,role[NAME]'
   
   .. end_tag
   
   
``subscribes``
   **Ruby Type:** Symbol, 'Chef::Resource[String]'

   .. tag resources_common_notification_subscribes
   
   A resource may listen to another resource, and then take action if the state of the resource being listened to changes. Specify a ``'resource[name]'``, the ``:action`` to be taken, and then the ``:timer`` for that action.
   
   .. end_tag
   

   .. tag resources_common_notification_timers
   
   A timer specifies the point during the chef-client run at which a notification is run. The following timers are available:
   
   ``:before``
      Specifies that the action on a notified resource should be run before processing the resource block in which the notification is located. 
   
   ``:delayed``
      Default. Specifies that a notification should be queued up, and then executed at the very end of the chef-client run.
   
   ``:immediate``, ``:immediately``
      Specifies that a notification should be run immediately, per resource notified.
   
   .. end_tag
   

   .. tag resources_common_notification_subscribes_syntax
   
   The syntax for ``subscribes`` is:
   
   .. code-block:: ruby
   
      subscribes :action, 'resource[name]', :timer
   
   .. end_tag
   
   
``tags``
   Use to specify the list of tags to be applied to the machine image. Any tag not specified in this list will be removed.

.. end_tag

