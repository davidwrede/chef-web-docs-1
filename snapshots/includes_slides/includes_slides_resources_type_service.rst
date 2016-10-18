.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.


A service that should be started:

.. code-block:: ruby
       
   service 'haproxy' do
     supports :restart => :true
     action [:enable, :start]
   end
