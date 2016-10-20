
.. tag server_replication_how_it_works

A daemon named **ec-syncd** runs on each of the replica instances of the Chef server and periodically polls the primary Chef server via the ``updated_since`` endpoint in the Chef server API. The **ec-syncd** daemon requests a list of objects that have been updated since the last successful synchronization time. If there are updates, the **ec-syncd** daemon then pulls down the updated data from the primary Chef server to the replica. 

.. image:: ../../images/chef_server_replication_sequence.png

.. end_tag

