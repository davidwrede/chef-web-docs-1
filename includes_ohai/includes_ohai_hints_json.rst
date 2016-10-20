
.. tag ohai_hints_json

If the hint file contains JSON content, it will be returned as a hash from the call to ``hint?``.

.. code-block:: javascript

   {
     "snow": true,
     "penguins": "many"
   }

.. code-block:: ruby

   antarctica_hint = hint?('antarctica')
   if antarctica_hint['snow']
     "There are #{antarctica_hint['penguins']} penguins here."
   else
     'There is no snow here, and penguins like snow.'
   end

The default directory in which hint files are located is ``/etc/chef/ohai/hints/``. Use the ``Ohai::Config[:hints_path]`` setting in the client.rb file to customize this location.

.. end_tag

