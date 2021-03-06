=====================================================
About |ohai|
=====================================================

.. include:: ../../includes_ohai/includes_ohai.rst

.. include:: ../../includes_ohai/includes_ohai_platforms.rst

Automatic Attributes
=====================================================
.. include:: ../../includes_ohai/includes_ohai_automatic_attribute.rst

**Get a list of automatic attributes for a node**

.. include:: ../../includes_ohai/includes_ohai_attribute_list.rst

.. note:: .. include:: ../../includes_notes/includes_notes_see_attributes_overview.rst

Attribute Persistence
-----------------------------------------------------
.. include:: ../../includes_node/includes_node_attribute_persistence.rst

Attribute Precedence
-----------------------------------------------------
.. include:: ../../includes_node/includes_node_attribute_precedence.rst

Whitelist Attributes
+++++++++++++++++++++++++++++++++++++++++++++++++++++
.. include:: ../../includes_node/includes_node_attribute_whitelist.rst

Default Plugins
=====================================================
.. include:: ../../includes_ohai/includes_ohai_plugins_default.rst

Custom Plugins
=====================================================
.. include:: ../../includes_ohai/includes_ohai_custom_plugin.rst

.. note:: See https://github.com/rackerlabs/ohai-plugins/tree/master/plugins for some great examples of custom |ohai| plugins.

.. warning:: The syntax for custom plugins changes significantly between |ohai| 6 and newer versions of |ohai|. This page is about newer plugins and `this page is about Ohai 6 plugins <https://docs.chef.io/release/ohai-6/>`_). While |company_name| has worked to ensure backwards compatibility for all |ohai| 6 plugins, a plan should be put in place to update the syntax for all |ohai| 6 plugins so they are usable with the new pattern. Once updated, please test and verify those plugins before running them in a production environment.

Syntax
-----------------------------------------------------
.. include:: ../../includes_ohai/includes_ohai_custom_plugin_syntax.rst

|dsl ohai| Methods
-----------------------------------------------------
.. include:: ../../includes_dsl_ohai/includes_dsl_ohai.rst

collect_data
+++++++++++++++++++++++++++++++++++++++++++++++++++++
.. include:: ../../includes_dsl_ohai/includes_dsl_ohai_method_collect_data.rst

Use a Mash
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. include:: ../../includes_dsl_ohai/includes_dsl_ohai_method_collect_data_mash.rst

Examples
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. include:: ../../includes_dsl_ohai/includes_dsl_ohai_method_collect_data_example.rst

require
+++++++++++++++++++++++++++++++++++++++++++++++++++++
.. include:: ../../includes_dsl_ohai/includes_dsl_ohai_method_require.rst

/common Directory
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. include:: ../../includes_dsl_ohai/includes_dsl_ohai_method_require_common.rst

Shared Methods
+++++++++++++++++++++++++++++++++++++++++++++++++++++
.. include:: ../../includes_dsl_ohai/includes_dsl_ohai_method_shared_methods.rst

Hints
-----------------------------------------------------
.. include:: ../../includes_ohai/includes_ohai_hints.rst

.. include:: ../../includes_ohai/includes_ohai_hints_json.rst

Log Entries
-----------------------------------------------------
.. include:: ../../includes_ohai/includes_ohai_custom_plugin_logs.rst

rescue
+++++++++++++++++++++++++++++++++++++++++++++++++++++
.. include:: ../../includes_ohai/includes_ohai_custom_plugin_logs_rescue.rst

Examples 
-----------------------------------------------------
The following examples show different ways of building |ohai| plugins.

collect_data Blocks
+++++++++++++++++++++++++++++++++++++++++++++++++++++
.. include:: ../../includes_ohai/includes_ohai_custom_plugin_example_multiple_collect_data_blocks.rst

Use a mixin Library
+++++++++++++++++++++++++++++++++++++++++++++++++++++
.. include:: ../../includes_ohai/includes_ohai_custom_plugin_example_use_mixin_library.rst

Get Kernel Values
+++++++++++++++++++++++++++++++++++++++++++++++++++++
.. include:: ../../includes_ohai/includes_ohai_custom_plugin_example_kernels.rst

|ohai| 6 vs. Newer Plugins
-----------------------------------------------------
.. include:: ../../includes_ohai/includes_ohai_migrate_plugins_6_to_7.rst

ohai Resource
=====================================================
.. include:: ../../includes_resources_common/includes_resources_common_generic.rst

.. include:: ../../includes_resources/includes_resource_ohai.rst

Syntax
-----------------------------------------------------
.. include:: ../../includes_resources/includes_resource_ohai_syntax.rst

Actions
-----------------------------------------------------
.. include:: ../../includes_resources/includes_resource_ohai_actions.rst

Attributes
-----------------------------------------------------
.. include:: ../../includes_resources/includes_resource_ohai_attributes.rst

Providers
-----------------------------------------------------
.. include:: ../../includes_resources/includes_resource_ohai_providers.rst

Examples
-----------------------------------------------------
|generic resource statement|

**Reload Ohai**

.. include:: ../../step_resource/step_resource_ohai_reload.rst

**Reload Ohai after a new user is created**

.. include:: ../../step_resource/step_resource_ohai_reload_after_create_user.rst


ohai Cookbook
=====================================================
.. include:: ../../step_ohai/step_ohai_download_cookbook.rst

Default Location
-----------------------------------------------------
.. include:: ../../step_ohai/step_ohai_plugin_change_path.rst

Upload Custom Plugins
-----------------------------------------------------
.. include:: ../../step_ohai/step_ohai_plugin_upload.rst

Add |ohai| to a Run-list
-----------------------------------------------------
.. include:: ../../step_ohai/step_ohai_add_to_run_list.rst


ohai Command Line Tool
=====================================================
.. include:: ../../includes_ctl_ohai/includes_ctl_ohai.rst

Options
-----------------------------------------------------
.. include:: ../../includes_ctl_ohai/includes_ctl_ohai_options.rst

Examples
-----------------------------------------------------
None.


|ohai| Settings in |client rb|
=====================================================

.. include:: ../../includes_config/includes_config_rb_ohai.rst

.. include:: ../../includes_config/includes_config_rb_ohai_settings.rst
