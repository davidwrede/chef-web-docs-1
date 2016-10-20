
.. tag ctl_chef_client_aix_requirements

The chef-client has the `same system requirements <https://docs.chef.io/chef_system_requirements.html#chef-client>`_ on the AIX platform as any other platform, with the following notes:

* Expand the file system on the AIX platform using ``chfs`` or by passing the ``-X`` flag to ``installp`` to automatically expand the logical partition (LPAR)
* The EN_US (UTF-8) character set should be installed on the logical partition prior to installing the chef-client

.. end_tag

