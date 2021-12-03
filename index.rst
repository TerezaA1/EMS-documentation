.. Energy managment portal documentation master file, created by
   sphinx-quickstart on Sun Aug  1 20:16:22 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


AMOS Documentation
=======================================

Welcome to the AMOS (Advanced Microgrid Operation System) documentation. Here you can find a user manual to all functions of the portal.


Introduction
------------
The AMOS is a web platform for viewing, oprating and parametrizing the microgrids. It shows real-time data from the site alongside forecasts and optimized operation of the microgrid. The microgrid can consist of loads, energy storage system and/or power generation plants. The portal has access to the central microgrid contoller, which is responsible for optimal operation and power flows of the system.

.. toctree::
   :maxdepth: 1
   :hidden:

   self


Getting started
~~~~~~~~~~~~~~~

Please go to `teslablueplanet.eu <https://teslablueplanet.eu/>`_ page, select the Energy managment portal and log in to the system with your email address and password:

.. image:: /images/ver02/index.*


It depends on the user role which functions are accessible. The system operator have access to all basic functionalities of the portal, can view telemetry data and foracasts, try different optimization scenarios and see simulation. The process admin has on top of the operator's rights also access to the microgrid setup options and battery model database.

This user manual provides description of the visual elements in the interface. The functions are documented as they appear on the left pane in the AMOS portal:

.. toctree::
   :maxdepth: 2

   content/ver02/microgrid
   content/ver02/forecasts
   content/ver02/digital_twin
