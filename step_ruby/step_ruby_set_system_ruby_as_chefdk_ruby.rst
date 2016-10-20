
.. tag ruby_set_system_ruby_as_chefdk_ruby

For many users of Chef, the Chef development kit version of Ruby that is included in the Chef development kit should be configured as the default version of Ruby.

#. Open a command window and enter the following:

   .. code-block:: bash

      $ which ruby

   which will return something like ``/usr/bin/ruby``.
#. To use the Chef development kit version of Ruby as the default Ruby, edit the ``$PATH`` and ``GEM`` environment variables to include paths to the Chef development kit. For example, on a machine that runs Bash, run:

   .. code-block:: bash

      echo 'eval "$(chef shell-init bash)"' >> ~/.bash_profile

   where ``bash`` and ``~/.bash_profile`` represents the name of the shell.

   If zsh is your preferred shell then run the following:

   .. code-block:: bash

    echo 'eval "$(chef shell-init zsh)"' >> ~/.zshrc

#. Run ``which ruby`` again. It should return ``/opt/chefdk/embedded/bin/ruby``.

.. note:: Using the Chef development kit-provided Ruby as your system Ruby is optional. This just depends on how you are using Ruby on your system. For many users, Ruby is primarily used for authoring Chef cookbooks and recipes. If that's true for you, then using the Chef development kit-provided Ruby as your system Ruby is recommended. But for other users who are already using tools like rbenv to manage Ruby versions, then that's OK too.


.. end_tag

