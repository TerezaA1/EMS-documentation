Telemetry
=========

Telemetry allows user to view real-time signals measured at the site and their historical records up to two months. A time window is customable.

.. image:: /images/telemetry_dates.PNG

All telemetry signals that are collected can be shown in the graph. User can choose from various items: data about battery storage, PV system, grid and other connected devices.

.. image:: /images/telemetry_signals.PNG

Data are visualized as time-series sequence with 1 minute resolution. On this graph can be seen daily profile of PV production with energy imported form the grid.

.. image:: /images/telemetry_plot.PNG

The interactive figure is produced with `Plotly graphing library <https://plotly.com/python/>`_ (as all figures in the EMS) that provide zooming, scaling and hovering options. Bar can be found in the top right corner.

.. image:: /images/plotly.PNG
   :align: center

It is possible to download the plot as a png. If needed, data can be shown in the table.

.. image:: /images/telemetry_table.PNG
