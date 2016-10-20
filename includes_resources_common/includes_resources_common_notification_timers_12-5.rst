
.. tag 5

A timer specifies the point during the chef-client run at which a notification is run. The following timers are available:

``:delayed``
   Default. Specifies that a notification should be queued up, and then executed at the very end of the chef-client run.

``:immediate``, ``:immediately``
   Specifies that a notification should be run immediately, per resource notified.



.. end_tag

