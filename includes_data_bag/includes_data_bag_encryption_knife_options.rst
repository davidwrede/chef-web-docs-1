
.. tag data_bag_encryption_knife_options

knife can encrypt and decrypt data bag items when the ``knife data bag`` subcommand is run with the ``create``, ``edit``, ``from file``, or ``show`` arguments and the following options:

.. list-table::
   :widths: 200 300
   :header-rows: 1

   * - Option
     - Description
   * - ``--secret SECRET``
     - The encryption key that is used for values contained within a data bag item. If ``secret`` is not specified, the chef-client looks for a secret at the path specified by the ``encrypted_data_bag_secret`` setting in the client.rb file.
   * - ``--secret-file FILE``
     - The path to the file that contains the encryption key.

.. end_tag

