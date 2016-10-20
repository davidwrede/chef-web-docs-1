
.. tag cookbooks_recipe_include_in_recipe

A recipe can include one (or more) recipes located in external cookbooks by using the ``include_recipe`` method. When a recipe is included, the resources found in that recipe will be inserted (in the same exact order) at the point where the ``include_recipe`` keyword is located.

The syntax for including a recipe is like this:

.. code-block:: ruby

   include_recipe 'recipe'

For example:

.. code-block:: ruby

   include_recipe 'apache2::mod_ssl'

If the ``include_recipe`` method is used more than once to include a recipe, only the first inclusion is processed and any subsequent inclusions are ignored.

.. end_tag

