
.. tag api_reporting_headers_x_ops_reporting_protocol_version

Use to specify the protocol version for the Reporting API. This header must be set to ``0.1.0``.

* A request to the Chef server API that does not include this header and the correct value will return a 404 response code.
* A request to the Chef server API that includes this header with an incorrect value will return a 406 reponse code.

If the protocol version is incorrect (or unspecified), the chef-client run will proceed normally, but Reporting data will not be collected for that chef-client run unless the ``enable_reporting_url_fatals`` setting is ``true`` in the client.rb file for that node.

.. end_tag

