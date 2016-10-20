
.. tag ctl_opscode_expander_example

For example, to view the aggregate queue backlog, enter the following:

.. code-block:: bash

   $ cd /opt/opscode/embedded/service/opscode-expander/
     export PATH=$PATH:/opt/opscode/bin:/opt/opscode/embedded/bin
     bin/opscode-expanderctl queue-depth

to return something similar to:

.. code-block:: bash

       total messages:       0
       average queue depth:  0.0
       max queue depth:      0
       min queue depth:      0


.. end_tag

