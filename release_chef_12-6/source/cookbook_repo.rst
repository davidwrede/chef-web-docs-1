.. THIS PAGE DOCUMENTS chef-client version 12.6

=====================================================
Cookbook Directories and Metadata
=====================================================

.. include:: ../../includes_chef_repo/includes_chef_repo_directory_cookbooks.rst

.. include:: ../../step_chef_repo/step_chef_repo_cookbooks_configure_settings.rst

Work with Cookbooks
=====================================================
Use the following |knife| subcommands to create, install, and/or download cookbooks.

Create
-----------------------------------------------------
.. include:: ../../step_knife/step_knife_cookbook_create.rst

Install
-----------------------------------------------------
.. include:: ../../step_knife/step_knife_cookbook_site_install.rst

Download
-----------------------------------------------------
.. include:: ../../step_knife/step_knife_cookbook_site_download.rst

About Cookbook Metadata
=====================================================

.. include:: ../../includes_cookbooks/includes_cookbooks_metadata.rst

Error Messages
-----------------------------------------------------
.. include:: ../../includes_cookbooks/includes_cookbooks_metadata_error_messages.rst

metadata.rb
-----------------------------------------------------
.. include:: ../../includes_cookbooks/includes_cookbooks_metadata.rst

.. include:: ../../includes_config/includes_config_rb_metadata.rst

Settings
+++++++++++++++++++++++++++++++++++++++++++++++++++++
This configuration file has the following settings:

``attribute``
   |metadata attributes|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_attribute.rst

``chef_version``
   |metadata rb chef_version|

   .. include:: ../../includes_config/includes_config_rb_metadata_settings_example_chef_version.rst

   .. note:: |metadata rb supermarket_not_visible|

``depends``
   |metadata rb depends|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_depends.rst

``description``
   |description cookbook|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_description.rst

``issues_url``
   |url cookbook_issues| |metadata rb supermarket_view_issues|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_issues_url.rst

``license``
   |license metadata_rb|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_license.rst

``long_description``
   |long description| 

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_long_description.rst

``maintainer``
   |maintainer|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_maintainer.rst

``maintainer_email``
   |maintainer email|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_maintainer_email.rst

``name``
   Required. |name cookbook|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_name.rst

``ohai_version``
   |metadata rb chef_version|

   .. include:: ../../includes_config/includes_config_rb_metadata_settings_example_ohai_version.rst

   .. note:: |metadata rb supermarket_not_visible|

``privacy``
   |metadata rb private|

``provides``
   |metadata rb provides|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_provides.rst

``recipe``
   |description recipe|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_recipe.rst

``source_url``
   |url cookbook_source| |metadata rb supermarket_view_source|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_source_url.rst

``supports``
   |metadata rb supports|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_supports.rst

``version``
   |version cookbook|

   .. include:: ../../includes_cookbooks/includes_cookbooks_metadata_settting_version.rst
