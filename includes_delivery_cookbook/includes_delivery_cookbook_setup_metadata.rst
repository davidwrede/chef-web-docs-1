
.. tag delivery_cookbook_setup_metadata

The metadata.rb for a ``build-cookbook`` is located at ``.delivery/build-cookbook/metadata.rb``. Update it to include:

.. code-block:: none

   depends 'delivery-truck'

This will ensure that the ``build-cookbook`` has a dependency on the ``delivery-truck`` cookbook.

.. end_tag

