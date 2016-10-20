
.. tag resource_machine_attributes

This resource has the following properties:
   
``admin``
   **Ruby Types:** TrueClass, FalseClass

   Use to specify whether the chef-client is an API client.
   
``allow_overwrite_keys``
   **Ruby Types:** TrueClass, FalseClass

   Use to overwrite the key on a machine when it is different from the key specified by ``source_key``.
   
``attribute``
   Use to specify an attribute, and then modify that attribute with the specified value. The following patterns may be used to specify the value.
	 
   .. code-block:: ruby

      attribute <name>, <value>
          
   .. code-block:: ruby

      attribute [<path>], <value>
          
   The following example will set attribute ``a`` to ``b``:

   .. code-block:: ruby

      attribute 'a', 'b'
          
   The following example will set attribute ``node['a']['b']['c']`` to ``d`` and will ignore attributes ``a.b.x``, ``a.b.y``, etc.:

   .. code-block:: ruby

      attribute %w[a b c], 'd'
          
   The following example is similar to ``%w[a b c], 'd'``:

   .. code-block:: ruby

      attribute 'a', { 'b' => { 'c' => 'd' } }

   Each modified attribute should be specified individually. This attribute should not be used in the same recipe as ``attributes``.
   
``attributes``
   Use to specify a Hash that contains all of the normal attributes to be applied to a machine. This attribute should not be used in the same recipe as ``attribute``.
   
``chef_config``
   **Ruby Type:** String

   Use to specify a string that contains extra configuration settings for a machine.
   
``chef_environment``
   The name of the environment.
   
``chef_server``
   **Ruby Type:** Hash

   The URL for the Chef server.
   
``complete``
   Use to specify if all of the normal attributes specified by this resource represent a complete specification of normal attributes for a machine. When ``true``, any attributes not specified will be reset to their default values. For example, if a **machine** resource is empty and sets ``complete`` to ``true``, all existing attributes will be reset:

   .. code-block:: ruby

      machine "foo" do
        complete "true"
      end
   
``converge``
   **Ruby Types:** TrueClass, FalseClass

   Use to manage convergence when used with the ``:create`` action. Set to ``false`` to prevent convergence. Set to ``true`` to force convergence. When ``nil``, the machine will converge only if something changes. Default value: ``nil``.
   
``driver``
   **Ruby Type:** Chef::Provisioning::Driver

   Use to specify the URL for the driver to be used for provisioning.
   
``files``
   **Ruby Type:** Hash

   A list of files to upload. Syntax: ``REMOTE_PATH => LOCAL_PATH_OR_HASH``.
       
   For example:
       
   .. code-block:: ruby
       
      files '/remote/path.txt' => '/local/path.txt'
       
   or:
       
   .. code-block:: ruby
       
      files '/remote/path.txt' => {
        :local_path => '/local/path.txt'
      }
       
   or:
       
   .. code-block:: ruby
       
      files '/remote/path.txt' => { :content => 'foo' }
   
``from_image``
   **Ruby Type:** String

   Use to specify an image created by the **machine_image** resource.
   
``ignore_failure``
   **Ruby Types:** TrueClass, FalseClass

   Continue running a recipe if a resource fails for any reason. Default value: ``false``.
   
``machine_options``
   **Ruby Type:** Hash

   A Hash that is specifies driver options.
   
``name``
   **Ruby Type:** String

   The name of the machine.
   
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
   
   
``ohai_hints``
   **Ruby Type:** Hash

   An Ohai hint to be set on the target node. For example: ``'ec2' => { 'a' => 'b' } creates file ec2.json with json contents { 'a': 'b' }``.
   
``private_key_options``
   **Ruby Type:** Hash

   Use to generate a private key of the desired size, type, and so on.
   
``public_key_format``
   **Ruby Type:** String

   Use to specify the format of a public key. Possible values: ``pem`` and ``der``. Default value: ``pem``.
   
``public_key_path``
   **Ruby Type:** String

   The path to a public key.
   
``raw_json``
   The machine as JSON data. For example:
       
   .. code-block:: javascript
   
      {
        "name": "node1",
        "chef_environment": "_default",
        "json_class": "Chef::Node",
        "automatic": {
          "languages": {
            "ruby": {
              ...
            },
          ...
        ...
      }
   
``recipe``
   Use to add a recipe to the run-list for a machine. Use this property multiple times to add multiple recipes to a run-list. Use this property along with ``role`` to define a run-list. The order in which the ``recipe`` and ``role`` properties are specified will determine the order in which they are added to the run-list. This property should not be used in the same recipe as ``run_list``. For example:
       
   .. code-block:: ruby
       
      recipe 'foo'
      role 'bar'
      recipe 'baz'
   
``remove_recipe``
   Use to remove a recipe from the run-list for the machine.
   
``remove_role``
   Use to remove a role from the run-list for the machine.
   
``remove_tag``
   Use to remove a tag.
   
``retries``
   **Ruby Type:** Integer

   The number of times to catch exceptions and retry the resource. Default value: ``0``.
   
``retry_delay``
   **Ruby Type:** Integer

   The retry delay (in seconds). Default value: ``2``.
   
``role``
   Use to add a role to the run-list for the machine. Use this property multiple times to add multiple roles to a run-list. Use this property along with ``recipe`` to define a run-list. The order in which the ``recipe`` and ``role`` properties are specified will determine the order in which they are added to the run-list. This property should not be used in the same recipe as ``run_list``. For example:
	 
   .. code-block:: ruby
       
      recipe 'foo'
      role 'bar'
      recipe 'baz'
   
``run_list``
   An array of strings that specifies the run-list to apply to a machine. This property should not be used in the same recipe as ``recipe`` and ``role``. For example:

   .. code-block:: ruby
       
      [ 'recipe[COOKBOOK::RECIPE]','COOKBOOK::RECIPE','role[NAME]' ]
   
``source_key``
   Use to copy a private key, but apply a different ``format`` and ``password``. Use in conjunction with ``source_key_pass_phrase``` and ``source_key_path``.
   
``source_key_pass_phrase``
   **Ruby Type:** String

   The pass phrase for the private key. Use in conjunction with ``source_key``` and ``source_key_path``.
   
``source_key_path``
   **Ruby Type:** String

   The path to the private key. Use in conjunction with ``source_key``` and ``source_key_pass_phrase``.
   
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
   
   
``tag``
   Use to add a tag.
   
``tags``
   Use to add one (or more) tags. This will remove any tag currently associated with the machine. For example: ``tags :a, :b, :c``.
   
``validator``
   **Ruby Types:** TrueClass, FalseClass

   Use to specify if the chef-client is a chef-validator.

.. end_tag

