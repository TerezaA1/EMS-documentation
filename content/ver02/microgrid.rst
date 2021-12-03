Microgrid
=========
After log in, the operator can preview and manage the selected microgrid.

.. image:: /images/ver02/side_navigation.PNG
   :align: center

|

Main navigation is in side bar menu, where each page has top navigation panel.

.. image:: /images/ver02/top_navigation.PNG

|

Overview
~~~~~~~~
Main screen shows online visualization of the power flows in the microgrid together with actual battery state of charge, PV power generation and other grid parameters.

.. image:: /images/ver02/overview.gif

|

In the topology editor, a user can modify what will be shown at this page.


Dashboard
~~~~~~~~~
Dashboard displays main system signals and battery data per current day.

.. image:: /images/ver02/dashboard.PNG

|

History
~~~~~~~~~
On the history page, the user can select any stored historical signals to plot in the graph during the chosen time period. Data are visualized as time-series sequence with custom sampling resolution.

.. image:: /images/ver02/history.PNG

|

The interactive figure is produced with `Plotly graphing library <https://plotly.com/python/>`_ (as other figures in the AMOS) that provide zooming, scaling and hovering options. Bar can be found in the top right corner.

.. image:: /images/plotly.PNG
   :align: center

|

It is possible to download the plot as a png. If needed, data can be shown in the table.

.. image:: /images/telemetry_table.PNG

|


Future
~~~~~~~~~
Here the operator can preview an optimal plan for energy dipatch how was predicted by the advanced controller at any time in the past. Graphs show forecasted production and consuption in the microgrid and planned action with battery.

.. image:: /images/ver02/future.PNG

|


Intelligence
~~~~~~~~~~~~
For SolarEdge inverter technology is available performance monitoring on PV panel level with further options of degradation evaluation and failure detection. In the graphical form is shown amount of energy produced by each PV module separately for selected day.

.. image:: /images/ver02/intelligence.PNG

|


Settings
~~~~~~~~
The system allowes to modify microgrid parameters regarding user permissions. The basic user can setup and change energy costs and limits for both - import and export. Maximum grid import is value of reserved capacity or other limit value that microgrid will respect and perform peak-shaving. If maximum export is set to 0, it is assumed that no energy (e.g. from PV system) is allowd to flow to the utility grid.

.. image:: /images/ver02/user_settings.PNG
   :align: center
   :width: 60%

|

The user can select multiple system functionalities that controller will perform. Difference between peak-shaving function and guarding grid limits is that peak-shaving aim is to lower peaks as much as possible, while guarding simply does not allow to exceed given limit.

.. image:: /images/ver02/functions.PNG

|

Operator has permissions to change battery parameters (nominal capacity, SoC and power limits) and options (when to prefer battery charging).

.. image:: /images/ver02/operator_settings.PNG
   :align: center
   :width: 60%

|

After every parameter change, it is possible to run virtual simulation to see consequences of such actions. Further, the admin user has access to the more advanced options including computation backend data.


Events
~~~~~~
The system logs every action and parameter change, which are displayed on the events page. Each action is assigned to the user and date.

.. image:: /images/ver02/events.PNG

|


Alerts
~~~~~~
Page for viewing system alerts and errors.
