.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.

A ``yaml`` |inspec resource| block declares the configuration data to be tested Assume the following |yaml| file:

.. code-block:: yaml

   name: foo
   array:
     - zero
     - one

This file can be queried using:

.. code-block:: ruby

   describe yaml do
     its('name') { should eq 'foo' }
     its(['array', 1]) { should eq 'one' }
   end

where

* ``name`` is a configuration setting in a |yaml| file
* ``should eq 'foo'`` tests a value of ``name`` as read from a |yaml| file versus the value declared in the test
