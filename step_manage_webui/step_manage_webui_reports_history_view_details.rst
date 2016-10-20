
.. tag manage_webui_reports_history_view_details

To view chef-client details:

#. Open the Chef management console.
#. Click **Reports**.
#. Click **Run History**.
#. Select the range of chef-client runs to show, the correct environment, and correct status.
#. Select a chef-client run.
#. Select the **Details** tab:

   .. image:: ../../images/step_manage_webui_reports_history_view_details.png

   where:

   .. list-table::
      :widths: 60 420
      :header-rows: 1
   
      * - Setting
        - Description
      * - ``Step``
        - The order in which resources were executed during the chef-client run.
      * - ``Type``
        - The type of resource. https://docs.chef.io/resource.html#resources
      * - ``Name``
        - A string that describes the action taken. For example, a log entry or the name of the service that is enabled.
      * - ``Action``
        - The action taken by the resource type.
      * - ``Duration``
        - The amount of time required to complete the action.
      * - ``Diff``
        - The difference between the current state and the previous state. This setting is available for files managed by the **cookbook_file**, **file**, **remote_file**, and **template** resources.
      * - ``Parameters``
        - Opens the **Run Details** dialog box, which lists all of the parameters on the node that were changed during the chef-client run.

.. end_tag

