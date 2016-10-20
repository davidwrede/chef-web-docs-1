
.. tag resource_ifconfig_update_static_ip_with_boot_protocol

.. To update a static IP address with a boot protocol*:

.. code-block:: ruby

   ifconfig "33.33.33.80" do
     bootproto "dhcp"
     device "eth1"
   end

will update the interface from ``static`` to ``dhcp``:

.. code-block:: none

   iface eth1 inet dhcp
     address 33.33.33.80

.. end_tag

