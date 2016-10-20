
.. tag config_rb_metadata_summary

A metadata.rb file is:

* Located at the top level of a cookbook's directory structure
* Compiled whenever a cookbook is uploaded to the Chef server or when the ``knife cookbook metadata`` subcommand is run, and then stored as JSON data
* Created automatically by knife whenever the ``knife cookbook create`` subcommand is run
* Edited using a text editor, and then re-uploaded to the Chef server as part of a cookbook upload

.. end_tag

