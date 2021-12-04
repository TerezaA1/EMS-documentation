.. Energy managment portal documentation master file, created by
   sphinx-quickstart on Sun Aug  1 20:16:22 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


AMOS Documentation
=======================================

Welcome to the AMOS (Advanced Microgrid Operation System) documentation. Here you can find a user manual to all functions of the portal.


Introduction
------------
The AMOS is a web platform for viewing, operating and parametrizing microgrids. It shows real-time data from the site alongside forecasts and optimized operation of the microgrid. The microgrid can consist of loads, energy storage systems and/or power generation plants. The portal has access to the central microgrid controller, which is responsible for optimal operation and power flows of the system.

.. toctree::
   :maxdepth: 1
   :hidden:

   self


Getting started
~~~~~~~~~~~~~~~

Please go to `teslablueplanet.eu <https://teslablueplanet.eu/>`_ page, select the Energy management portal and log in to the system with your email address and password:

.. image:: /images/ver02/index.*


It depends on the user role which functions are accessible. The system operator has access to all basic functionalities of the portal, can view telemetry data and forecasts, try different optimization scenarios and see the simulation. The process admin has on top of the operator's rights also access to the microgrid setup options and battery model database.

This user manual provides a description of the visual elements in the web interface. The functions are documented as they appear on the left pane in the AMOS portal:

.. toctree::
   :maxdepth: 2

   content/microgrid
   content/forecasts
   content/digital_twin
   content/commissioning
   content/database
