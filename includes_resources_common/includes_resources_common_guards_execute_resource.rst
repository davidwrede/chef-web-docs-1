
.. tag resources_common_guards_execute_resource

When using the ``not_if`` and ``only_if`` guards with the **execute** resource, the current working directory property (``cwd``) is **not** inherited from the resource. For example:

.. code-block:: ruby

   execute 'bundle install' do
     cwd '/myapp'
     not_if 'bundle check' # This is not run inside /myapp
   end

.. end_tag

