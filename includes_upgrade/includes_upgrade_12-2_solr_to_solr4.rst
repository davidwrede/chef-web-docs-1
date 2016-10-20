
.. tag 2_solr_to_solr4

Chef server version 12 is upgraded to Apache Solr 4. If Apache Solr options were added to the private-chef.rb file under ``opscode_solr`` for Enterprise Chef, those configuration options are now stored under ``opscode_solr4`` in the chef-server.rb file for Chef server version 12.

Some ``opscode_solr`` settings are imported automatically, such as heap, new size, and Java options, but many settings are ignored. If your Enterprise Chef configuration is highly tuned for Apache Solr, review `these configuration settings <https://docs.chef.io/config_rb_server_optional_settings.html#opscode-solr4>`__ before re-tuning Apache Solr for Chef server version 12.

.. end_tag

