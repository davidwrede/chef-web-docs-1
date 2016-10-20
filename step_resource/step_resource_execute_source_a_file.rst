
.. tag resource_execute_source_a_file

The **execute** resource cannot be used to source a file (e.g. ``command 'source filename'``). The following example will fail because ``source`` is not an executable:

.. code-block:: ruby

   execute 'foo' do
     command 'source /tmp/foo.sh'
   end

Instead, use the **script** resource or one of the **script**-based resources (**bash**, **csh**, **perl**, **python**, or **ruby**). For example:

.. code-block:: ruby

   bash 'foo' do
     code 'source /tmp/foo.sh'
   end

.. end_tag

