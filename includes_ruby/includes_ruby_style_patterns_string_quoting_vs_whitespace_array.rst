
.. tag ruby_style_patterns_string_quoting_vs_whitespace_array

When ``%w`` syntax uses a variable, such as ``|foo|``, double quoted strings should be used.

Right:

.. code-block:: ruby

   %w{openssl.cnf pkitool vars Rakefile}.each do |foo|
     template "/etc/openvpn/easy-rsa/#{foo}" do
       source "#{foo}.erb"
       ...
     end
   end

Wrong:

.. code-block:: ruby

   %w{openssl.cnf pkitool vars Rakefile}.each do |foo|
     template '/etc/openvpn/easy-rsa/#{foo}' do
       source '#{foo}.erb'
       ...
     end
   end

.. end_tag

