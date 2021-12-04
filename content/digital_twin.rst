Digital Twin
======================

Optimization algorithm is repeatedly running on the microgrid controller. Objective of the optimal control is to minimize operational cost of the whole system, considering given technical constraints. On this page, the user see a digital twin of the microgid, can change parameters, select functionalities and observe changes in the simulation.

Parameters
~~~~~~~~~~

It is possible to try different forecasting services that produce different results, whichcan be further modified.

.. image:: /images/ver02/services.PNG

|

Predictive control algorithm optimize system performance over receding horizon of given length sampled into time intervals, which are also customable.

.. image:: /images/ver02/opt_horizon.PNG

|

Here is option to choose from external optimization solvers. Solvers are responsible for computation and they may differ in the speed of finding a solution. SoC formulation is related to how the battery constraints are formulated. Convex relaxation keeps optimization problem in linear form, which is easiliy solvable. Binary formulation introduce binary variables necessary because of nonlinear nature of the battery loses, turning the optimization into the mixed-integer programming problem. This makes results more precise, but comes with higher computational costs.

.. image:: /images/ver02/opt_solvers.PNG

|

One of the main functionalities of the battery storage in the microgrid is peak-shaving. The microgrid controller guard given capacity cap. The battery will be discharged above the cap to reduce the grid import, if has enough energy. The incomming peaks are predicted with :ref:`load forecasting <load-forecast>` model, which is trained on history data.

It depends on grid connection whether feed-ins and selling energy into the utility grid are allowed, this parameter is configurable and fully optional. It is possible to adjust feed-in tariffs, bonuses and track the reference, if desired.

.. image:: /images/ver02/grid_connection.PNG

|

Battery parameters (capacity, power, efficiencies) may be mannualy adjusted. Minimum and maximum state of charge (SoC) restrict microgrid controller from using battery above the limits. The limits should be set to respect the battery depth of discharge (DoD). The limits may be violated if the system comes to a situation with no other way out, for example when the battery has no capacity left to provide peak-shaving.

At the bottom is checkbox, which if selected allowes battery to be charged form the grid and increase a site consumption. Otherwise the battery can be charged only from the local energy sources.

.. image:: /images/ver02/opt_battery.PNG

|

The microgrid can also contain and utilize a combined heat and power (CHP) unit. All necessary technical (power, range, constraints) and economical (prices, costs) parameters of the CHP unit are adjusted here.

.. image:: /images/ver02/opt_CHP.PNG

|

Select desired functionalities that microgid will perform, it is possible to try different combinations to see their impact in the simulation.

.. image:: /images/ver02/opt_functionalities.PNG

|

Choose method how the microgrid provides flexibility.

.. image:: /images/ver02/opt_flexibility.PNG

|

Before running optimization, the user can check and adjust current measured values of PV, load and battery.

.. image:: /images/ver02/opt_measurements.PNG

|


Visualization
~~~~~~~~~~~~~

The results of optimal power schedule are visualised in the graphs. First plot shows grid import/export compared with load demand profile, together with other power sources (PV, CHP). Red dashed line indicates capacity cap (other color legend appears on the right side). The bottom plot shows which power sources and to what extent will be used to provide energy for demand.

.. image:: /images/opt_plot_load.PNG

|

Battery power flows are shown in th bar graph, where charging intervals are positive and discharging are negative. At the bottom is state of charge (green) with upper and lower bounds. Hover over the figures to show data values or look at the table below.

.. image:: /images/opt_plot_battery.PNG

|


