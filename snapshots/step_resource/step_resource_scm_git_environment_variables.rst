.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.

.. To pass in environment variables:

.. code-block:: ruby

   git '/opt/mysources/couch' do
     repository 'git://git.apache.org/couchdb.git'
     revision 'master'
     environment  { 'VAR' => 'whatever' }
     action :sync
   end
