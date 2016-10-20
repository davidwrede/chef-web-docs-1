
.. tag server_security_ssl_cert_custom

The Chef server can be configured to use SSL certificates by adding the following settings to the server configuration file:

.. list-table::
   :widths: 200 300
   :header-rows: 1

   * - Setting
     - Description
   * - ``nginx['ssl_certificate']``
     - The SSL certificate used to verify communication over HTTPS.
   * - ``nginx['ssl_certificate_key']``
     - The certificate key used for SSL communication.

and then setting their values to define the paths to the certificate and key.

.. end_tag

