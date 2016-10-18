=====================================================
knife cookbook site 
=====================================================

.. include:: ../../includes_api_cookbooks_site/includes_api_cookbooks_site.rst

.. include:: ../../includes_knife/includes_knife_site_cookbook.rst

.. warning:: .. include:: ../../includes_notes/includes_notes_knife_cookbook_site_use_devkit_berkshelf.rst

.. note:: .. include:: ../../includes_knife/includes_knife_common_see_common_options_link.rst

download
=====================================================
.. include:: ../../includes_knife/includes_knife_site_cookbook_download.rst

Syntax
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_download_syntax.rst

Options
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_download_options.rst

.. note:: .. include:: ../../includes_knife/includes_knife_common_see_all_config_options.rst

Examples
-----------------------------------------------------
The following examples show how to use this knife subcommand:

**Download a cookbook**

.. include:: ../../step_knife/step_knife_site_cookbook_download.rst

install
=====================================================
.. include:: ../../includes_knife/includes_knife_site_cookbook_install.rst

Syntax
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_install_syntax.rst

Options
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_install_options.rst

.. note:: .. include:: ../../includes_knife/includes_knife_common_see_all_config_options.rst

Examples
-----------------------------------------------------
The following examples show how to use this knife subcommand:

**Install a cookbook**

.. include:: ../../step_knife/step_knife_site_cookbook_install.rst

list
=====================================================
.. include:: ../../includes_knife/includes_knife_site_cookbook_list.rst

Syntax
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_list_syntax.rst

Options
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_list_options.rst

Examples
-----------------------------------------------------
The following examples show how to use this knife subcommand:

**View a list of cookbooks**

.. include:: ../../step_knife/step_knife_site_cookbook_list.rst

search
=====================================================
.. include:: ../../includes_knife/includes_knife_site_cookbook_search.rst

Syntax
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_search_syntax.rst

Options
-----------------------------------------------------
This command does not have any specific options.

Examples
-----------------------------------------------------
The following examples show how to use this knife subcommand:

**Search for cookbooks**

.. include:: ../../step_knife/step_knife_site_cookbook_search.rst

share
=====================================================
.. include:: ../../includes_knife/includes_knife_site_cookbook_share.rst

Syntax
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_share_syntax.rst

Options
-----------------------------------------------------
This argument has the following options:

``CATEGORY``
   The cookbook category: ``"Databases"``, ``"Web Servers"``, ``"Process Management"``, ``"Monitoring & Trending"``, ``"Programming Languages"``, ``"Package Management"``, ``"Applications"``, ``"Networking"``, ``"Operating Systems & Virtualization"``, ``"Utilities"``, or ``"Other"``.

``-n``, ``--dry-run``
   Take no action and only print out results. Default: ``false``.

``-o PATH:PATH``, ``--cookbook-path PATH:PATH``
   The directory in which cookbooks are created. This can be a colon-separated path.

.. note:: .. include:: ../../includes_knife/includes_knife_common_see_all_config_options.rst

Examples
-----------------------------------------------------
The following examples show how to use this knife subcommand:

**Share a cookbook**

.. include:: ../../step_knife/step_knife_site_cookbook_share.rst


show
=====================================================
.. include:: ../../includes_knife/includes_knife_site_cookbook_show.rst

Syntax
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_show_syntax.rst

Options
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_show_options.rst

Examples
-----------------------------------------------------
The following examples show how to use this knife subcommand:

**Show cookbook data**

.. include:: ../../step_knife/step_knife_site_cookbook_show.rst

**Show cookbook data as JSON**

.. include:: ../../step_knife/step_knife_site_cookbook_show_json.rst


unshare
=====================================================
.. include:: ../../includes_knife/includes_knife_site_cookbook_unshare.rst

Syntax
-----------------------------------------------------
.. include:: ../../includes_knife/includes_knife_site_cookbook_unshare_syntax.rst

Options
-----------------------------------------------------
This command does not have any specific options.

Examples
-----------------------------------------------------
The following examples show how to use this knife subcommand:

**Unshare a cookbook**

.. include:: ../../step_knife/step_knife_site_cookbook_unshare.rst

**Unshare a cookbook version**

To unshare cookbook version ``0.10.0`` for the ``getting-started`` cookbook, enter:

.. code-block:: bash

   $ knife cookbook site unshare "getting-started/version/0.10.0"
