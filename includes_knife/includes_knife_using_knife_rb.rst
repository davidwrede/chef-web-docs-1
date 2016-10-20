
.. tag knife_using_knife_rb

In addition to the default settings in a knife.rb file, there are other subcommand-specific settings that can be added. When a subcommand is run, knife will use:

#. A value passed via the command-line
#. A value contained in the knife.rb file
#. The default value

A value passed via the command line will override a value in the knife.rb file; a value in a knife.rb file will override a default value.


.. end_tag

