
.. tag resource_batch_attributes

This resource has the following properties:

``architecture``
   **Ruby Type:** Symbol

   The architecture of the process under which a script is executed. If a value is not provided, the chef-client defaults to the correct value for the architecture, as determined by Ohai. An exception is raised when anything other than ``:i386`` is specified for a 32-bit process. Possible values: ``:i386`` (for 32-bit processes) and ``:x86_64`` (for 64-bit processes).

``code``
   **Ruby Type:** String

   A quoted (" ") string of code to be executed.

``command``
   **Ruby Types:** String, Array

   The name of the command to be executed.

``creates``
   **Ruby Type:** String

   Prevent a command from creating a file when that file already exists.

``cwd``
   **Ruby Type:** String

   The current working directory from which a command is run.

``flags``
   **Ruby Type:** String

   One or more command line flags that are passed to the interpreter when a command is invoked.

``group``
   **Ruby Types:** String, Integer

   The group name or group ID that must be changed before running a command.

``guard_interpreter``
   **Ruby Type:** Symbol

   Default value: ``:batch``. When this property is set to ``:batch``, the 64-bit version of the cmd.exe shell will be used to evaluate strings values for the ``not_if`` and ``only_if`` properties. Set this value to ``:default`` to use the 32-bit version of the cmd.exe shell.

``ignore_failure``
   **Ruby Types:** TrueClass, FalseClass

   Continue running a recipe if a resource fails for any reason. Default value: ``false``.

``interpreter``
   **Ruby Type:** String

   The script interpreter to use during code execution. Changing the default value of this property is not supported.

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
   

``provider``
   **Ruby Type:** Chef Class

   Optional. Explicitly specifies a provider.

``retries``
   **Ruby Type:** Integer

   The number of times to catch exceptions and retry the resource. Default value: ``0``.

``retry_delay``
   **Ruby Type:** Integer

   The retry delay (in seconds). Default value: ``2``.

``returns``
   **Ruby Types:** Integer, Array

   The return value for a command. This may be an array of accepted values. An exception is raised when the return value(s) do not match. Default value: ``0``.

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
   

``timeout``
   **Ruby Types:** Integer, Float

   The amount of time (in seconds) a command is to wait before timing out. Default value: ``3600``.

``user``
   **Ruby Types:** String, Integer

   A user name or identifier that must be changed before running a command.

.. note:: See http://technet.microsoft.com/en-us/library/bb490880.aspx for more information about the cmd.exe interpreter.

.. end_tag

