
.. tag search_key_nested_starting_with

To find all IP address that are on the same network, enter the following:

.. code-block:: bash

   $ knife search node 'network_interfaces__addresses:192.168*'

where ``192.168*`` is the network address for which the search will be run.

.. end_tag

