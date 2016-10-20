
.. tag api_chef_server_endpoint_keys_clients_get

The ``GET`` method is used to retrieve all of the named client's key identifiers, associated URIs, and expiry states.

This method has no parameters.

**Request**

.. code-block:: none

   GET /organizations/NAME/clients/CLIENT/keys

**Response**

The response is similar to:

.. code-block:: javascript

   [
     { "name" : "default",
                "uri" : "https://chef.example/organizations/example/clients/client1/keys/default",
                "expired" : false },
     { "name" : "key1",
                "uri" : "https://chef.example/organizations/example/clients/client1/keys/key1",
                "expired" : true }
   ]

**Response Codes**

.. list-table::
   :widths: 200 300
   :header-rows: 1

   * - Response Code
     - Description
   * - ``200``
     - OK. The request was successful.
   * - ``401``
     - Unauthorized. The user or client who made the request could not be authenticated. Verify the user/client name, and that the correct key was used to sign the request.
   * - ``403``
     - Forbidden. The user who made the request is not authorized to perform the action.
   * - ``404``
     - Not found. The requested object does not exist.

.. end_tag

