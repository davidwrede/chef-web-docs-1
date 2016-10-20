
.. tag chef_repo_git_master_sync

Use the following steps to synchronize the master branch. 

#. Run:
    
   .. code-block:: bash

      $ git fetch chef

#. And then run:

   .. code-block:: bash

      $ git rebase chef/master master

   .. note:: Use ``rebase`` instead of ``merge`` to ensure that a linear history is maintained that does not include unnecessary merge commits. ``rebase`` will also rewind, apply, and then reapply commits to the ``master`` branch.

.. end_tag

