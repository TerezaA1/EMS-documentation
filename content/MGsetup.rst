Microgrid Setup
===============

Only users with admin status have permission to the microgrid setup. It is possible to edit microgrid data.

.. image:: /images/setup_edit.PNG
   :align: center
   :scale: 70 %

Each microgrid is composed of unit elements (storage, PV system, CHP unit). Battery model can be selected from the :doc:`database </content/battery>`.

.. image:: /images/setup_battery.PNG
   :align: center
   :scale: 70 %

Installed PV panels are grouped into the sets with same properties, shown in the editable table. Exact PV parameters are necessary for forecasts.

.. image:: /images/setup_PV.PNG

Grid connection parametres and costs are set up here.

.. image:: /images/setup_grid.PNG

Local controller setup allows to adjust polling intervals from telemetry and external services. ComAp communication setup. Security tokens and public keys are displayed.

.. image:: /images/setup_controller.PNG
   :align: center
   :scale: 70 %

.. image:: /images/setup_comap.PNG
   :align: center
   :scale: 70 %

Forecast services page permits user to set up weather, PV power and local load predictions parameters, such as polling intervals and number of days to forecast. It is possible to choose from available external service providers.

.. image:: /images/setup_forecast.PNG
   :align: center
   :scale: 70 %