
.. tag server_ha_external_postgresql

The following diagram highlights the specific changes that occur when PostgreSQL is configured and managed independently of the Chef server configuration.

.. image:: ../../images/server_components_postgresql.svg
   :width: 500px

The following table describes the components in an external PostgreSQL configuration that are different from the default configuration of the Chef server:

.. list-table::
   :widths: 60 420
   :header-rows: 1

   * - Component
     - Description
   * - Chef Server
     - The Chef server configuration file is updated to point to an independently configured set of servers for PostgreSQL.
   * - PostgreSQL
     - .. tag chef_server_component_postgresql
       
       PostgreSQL is the data storage repository for the Chef server.
       
       .. end_tag
       

       This represents the independently configured set of servers that are running PostgreSQL and are configured to act as the data store for the Chef server.

.. end_tag

