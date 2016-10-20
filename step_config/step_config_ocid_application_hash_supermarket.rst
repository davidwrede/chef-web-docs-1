
.. tag config_ocid_application_hash_supermarket

To define OAuth 2 information for Chef Supermarket, create a Hash similar to:

   .. code-block:: ruby

      oc_id['applications'] ||= {}
      oc_id['applications']['supermarket'] = {
        'redirect_uri' => 'https://supermarket.mycompany.com/auth/chef_oauth2/callback'
      }

.. end_tag

