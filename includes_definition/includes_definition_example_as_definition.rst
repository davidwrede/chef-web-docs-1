
.. tag definition_example_as_definition

The following definition processes unique hostnames and ports, passed on as parameters:
 		 
.. code-block:: ruby
 		 
   define :host_porter, :port => 4000, :hostname => nil do
     params[:hostname] ||= params[:name]

     directory '/etc/#{params[:hostname]}' do
       recursive true
     end

     file '/etc/#{params[:hostname]}/#{params[:port]}' do
       content 'some content'
     end
   end

.. end_tag

