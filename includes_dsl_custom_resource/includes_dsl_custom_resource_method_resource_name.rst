
.. tag dsl_custom_resource_method_resource_name

Use the ``resource_name`` method at the top of a custom resource to declare a custom name for that resource. For example:

.. code-block:: ruby

   resource_name :custom_name

where ``:custom_name`` is the resource name as it may be used in a recipe. For example, a cookbook named ``website`` and a custom resource file named ``httpd`` is by default used in a recipe with ``website_httpd``. If ``:custom_name`` is ``web_httpd`` then it may be used like this:

.. code-block:: ruby

   web_httpd 'name' do
     # properties
   end

.. end_tag

