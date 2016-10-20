
.. tag dsl_custom_resource_method_property

Use the ``property`` method to define properties for the custom resource. The syntax is:

.. code-block:: ruby

   property :name, ruby_type, default: 'value'

where

* ``:name`` is the name of the property
* ``ruby_type`` is the Ruby type, such as ``String``, ``Integer``, ``TrueClass``, or ``FalseClass``
* ``default: 'value'`` is the default value loaded into the resource

For example, the following properties define ``username`` and ``password`` properties with no default values specified:

.. code-block:: ruby

   property :username, String
   property :password, String

.. end_tag

