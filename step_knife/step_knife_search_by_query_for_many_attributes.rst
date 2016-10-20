
.. tag knife_search_by_query_for_many_attributes

To build a search query to use more than one attribute, use an underscore (``_``) to separate each attribute. For example, the following query will search for all nodes running a specific version of Ruby:

.. code-block:: bash

	$ knife search node "languages_ruby_version:1.9.3"

.. end_tag

