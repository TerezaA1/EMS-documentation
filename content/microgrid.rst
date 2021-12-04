Microgrid
=========
After logging in, the operator can preview and manage the selected microgrid.

.. image:: /images/ver02/side_navigation.PNG
   :align: center

|

The main navigation is in the sidebar menu, where each page has a top navigation panel.

.. image:: /images/ver02/top_navigation.PNG

|

Overview
~~~~~~~~
The main screen shows online visualization of the power flows in the microgrid together with the actual battery state of charge, PV power generation and other grid parameters. In the topology editor, the user can modify what will be shown on this page.

.. image:: /images/ver02/overview.gif

|


Dashboard
~~~~~~~~~
Dashboard displays main system signals and battery data per current day.

.. image:: /images/ver02/dashboard.PNG

|

History
~~~~~~~~~
On the history page, the user can select any stored historical signals to plot in the graph during the chosen time period. Data are visualized as a time-series sequence with custom sampling resolution.

.. image:: /images/ver02/history.PNG

|

The interactive figure is produced with `Plotly graphing library <https://plotly.com/python/>`_ (as other figures in the AMOS) that provide zooming, scaling and hovering options. The bar can be found in the top right corner.

.. image:: /images/plotly.PNG
   :align: center

|

It is possible to download the plot as a png. If needed, data can be shown in the table.

.. image:: /images/telemetry_table.PNG

|


Future
~~~~~~~~~
Here the operator can preview an optimal plan for energy dispatch how was predicted by the advanced controller at any time in the past. Graphs show forecasted production and consumption in the microgrid and planned action with the battery.

.. image:: /images/ver02/future.PNG

|


Intelligence
~~~~~~~~~~~~
For SolarEdge inverter technology is available performance monitoring on PV panel level with further options of degradation evaluation and failure detection. In the graphical form is shown the amount of energy produced by each PV module separately for the selected day.

.. image:: /images/ver02/intelligence.PNG

|


Settings
~~~~~~~~
The system allows modification of microgrid parameters regarding user permissions. The basic user can set up and change energy costs and limits for both - import and export. Maximum grid import is the value of reserved capacity or other limit value that microgrid will respect and perform peak-shaving. If maximum export is set to 0, it is assumed that no energy (e.g. from PV system) is allowed to flow to the utility grid.

.. image:: /images/ver02/user_settings.PNG
   :align: center
   :width: 60%

|

The user can select multiple system functionalities that the controller will perform. The difference between peak-shaving function and guarding grid limits is that peak-shaving aim is to lower peaks as much as possible while guarding simply does not allow to exceed given limit.

.. image:: /images/ver02/functions.PNG

|

The operator has permission to change battery parameters (nominal capacity, SoC and power limits) and options (when to prefer battery charging).

.. image:: /images/ver02/operator_settings.PNG
   :align: center
   :width: 60%

|

After every parameter change, it is possible to run a virtual simulation to see the consequences of such actions. Further, the admin user has access to the more advanced options including computation backend data.


Events
~~~~~~
The system logs every action and parameter change, which are displayed on the events page. Each action is assigned to the user and date.

.. image:: /images/ver02/events.PNG

|


Alerts
~~~~~~
A page for viewing system alerts and errors.
