
.. tag resource_scm_git_environment_variables

.. To pass in environment variables:

.. code-block:: ruby

   git '/opt/mysources/couch' do
     repository 'git://git.apache.org/couchdb.git'
     revision 'master'
     environment  { 'VAR' => 'whatever' }
     action :sync
   end

.. end_tag

