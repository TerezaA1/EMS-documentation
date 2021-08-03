Real-Time Optimization
======================

Optimization algorithm is repeatedly running on the microgrid controller. On this page, the user see a digital twin of the microgid, can change parameters, select functionalities and observe changes in the simulation. Objective of the optimal control is to minimize operational cost of the whole system, considering given technical constraints.

Parameters
~~~~~~~~~~

Predictive control optimize system performance over receding horizon of given length sampled into time intervals, which are also customable.

.. image:: /images/opt_horizon.PNG

Here is option to choose from external optimization solvers. Solvers are responsible for computation and they may differ in the speed of finding a solution. SoC formulation is related to how the battery constraints are formulated. Convex relaxation keeps optimizarion problem in linear form, which is easiliy solvable. Binary formulation introduce binary variables necessary because of nonlinear nature of the battery loses, turning the optimization into the mixed-integer programming problem. This makes results more precise, but comes with higher computational costs.

.. image:: /images/opt_solver.PNG

Battery parameters (capacity, power, efficiencies) may be mannualy adjusted. Minimum and maximum state of charge (SoC) restrict microgrid controller from using battery above the limits. The limits should be set to respect the battery depth of discharge (DoD). The limits may be violated if the system comes to a situation with no other way out, for example when the battery has no capacity left to provide peak-shaving.

At the bottom is checkbox, which if selected allowes battery to be charged form the grid and increase a site consumption. Otherwise the battery can be charged only from the local energy sources.

.. image:: /images/opt_battery.PNG

Feed

.. image:: /images/opt_feedin.PNG



.. image:: /images/opt_CHP.PNG



.. image:: /images/opt_cap.PNG



.. image:: /images/opt_flex.PNG



.. image:: /images/opt_measurement.PNG


Visualization
~~~~~~~~~~~~~