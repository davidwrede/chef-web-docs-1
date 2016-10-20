
.. tag resource_package_chef_gem_attribute_compile_time

.. This topic is hooked into client.rb topics, starting with 12.1, in addition to the resource reference pages.

To suppress warnings for cookbooks authored prior to chef-client 12.1, use a ``respond_to?`` check to ensure backward compatibility. For example:

.. code-block:: ruby

   chef_gem 'aws-sdk' do
     compile_time false if respond_to?(:compile_time)
   end

.. end_tag

