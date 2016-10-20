
.. tag server_firewalls_and_ports_tiered

For back-end servers in a tiered Chef server installation, ensure that ports marked as external (marked as ``yes`` in the **External** column) are open and accessible via any firewalls that are in use:

.. list-table::
   :widths: 60 420 60
   :header-rows: 1

   * - Port
     - Service Name, Description
     - External
   * - 80, 443, 9683
     - **nginx**

       .. tag server_services_nginx
       
       The **nginx** service is used to manage traffic to the Chef server, including virtual hosts for internal and external API request/response routing, external add-on request routing, and routing between front- and back-end components.
       
       .. end_tag
       

       .. note:: Port 9683 is used to internally load balance the **oc_bifrost** service.
     - yes
   * - 9463
     - **oc_bifrost**

       .. tag server_services_bifrost
       
       The **oc_bifrost** service ensures that every request to view or manage objects stored on the Chef server is authorized.
       
       .. end_tag
       
     - 
   * - 8983
     - **opscode-solr4**

       .. tag server_services_solr4
       
       The **opscode-solr4** service is used to create the search indexes used for searching objects like nodes, data bags, and cookbooks. (This service ensures timely search results via the Chef server API; data that is used by the Chef platform is stored in PostgreSQL.)
       
       .. end_tag
       
     - 
   * - 5432
     - **postgresql**

       .. tag server_services_postgresql
       
       The **postgresql** service is used to store node, object, and user data.
       
       .. end_tag
       
     - 
   * - 5672, 15672
     - **rabbitmq**

       .. tag server_services_rabbitmq
       
       The **rabbitmq** service is used to provide the message queue that is used by the Chef server to get search data to Apache Solr so that it can be indexed for search. When Chef Analytics is confiugred, the **rabbitmq** service is also used to send data from the Chef server to the Chef Analytics server.
       
       .. end_tag
       
     - 
   * - 16379
     - **redis_lb**

       .. tag server_services_redis
       
       Key-value store used in conjunction with Nginx to route requests and populate request data used by the Chef server.
       
       .. end_tag
       
     - 
   * - 4321
     - **bookshelf**

       .. tag server_services_bookshelf
       
       The **bookshelf** service is an Amazon Simple Storage Service (S3)-compatible service that is used to store cookbooks, including all of the files---recipes, templates, and so on---that are associated with each cookbook.
       
       .. end_tag
       
     - 
   * - 8000
     - **opscode-erchef**

       .. tag server_services_erchef
       
       The **opscode-erchef** service is an Erlang-based service that is used to handle Chef server API requests to the following areas within the Chef server:
       
       * Cookbooks
       * Data bags
       * Environments
       * Nodes
       * Roles
       * Sandboxes
       * Search
       
       .. end_tag
       
     -

.. end_tag

