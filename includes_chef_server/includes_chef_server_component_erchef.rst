
.. tag chef_server_component_erchef

Erchef is a complete rewrite of the core API for the Chef server, which allows it to be faster and more scalable than previous versions. The API itself is still compatible with the original Ruby-based Chef server, which means that cookbooks and recipes that were authored for the Ruby-based Chef server will continue to work on the Erlang-based Chef server. The chef-client is still written in Ruby.

.. note:: Even though the Chef server is authored in Erlang, writing code in Erlang is NOT a requirement for using Chef.

.. end_tag

