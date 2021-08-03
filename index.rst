.. Energy managment portal documentation master file, created by
   sphinx-quickstart on Sun Aug  1 20:16:22 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


Energy Managment Portal's Documentation
=======================================

Welcome to Energy managment portal's documentation. Here you can find a user manual to all functions of the portal.


Introduction
------------
The energy managment system (EMS) is a platform for viewing, oprating and parametrizing the microgrids. It shows real-time data from the site alongside forecasts and optimized operation of the microgrid. The microgrid can consist of loads, energy storage system and/or power generation plants. The portal has access to the central microgrid contoller, which is responsible for optimal operation and power flows of the system.

.. toctree::
   :maxdepth: 1
   :hidden:

   self


Getting started
~~~~~~~~~~~~~~~

Please go to `teslablueplanet.eu <https://teslablueplanet.eu/>`_ and log in into the system with your email address and password:

.. image:: /images/login.*

It depends on the user role which functions are accessible. The system operator have access to all basic functionalities of the portal, can view telemetry data and foracasts, try different optimization scenarios and see simulation. The process admin has on top of the operator's rights also access to microgrid setup and battery models database with the option of parametrization.

The functions are documented as they appear on the left pane in the EMS portal:

.. toctree::
   :maxdepth: 1

   content/microgrid_overview
   content/PVpanels
   content/telemetry
   content/forecasts
   content/RTO
   content/DAP
   content/MGsetup
   content/battery