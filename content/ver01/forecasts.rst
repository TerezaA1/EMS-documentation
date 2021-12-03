Forecasts
=========

The forecasts page shows all necessary predictions. Microgrid's energy managment system uses predictive control for optimal operation of the system and must utilize power forecasts. They are also used for a :doc:`day-ahead planning </content/DAP>`.


Weather Forecasts
~~~~~~~~~~~~~~~~~

Weather forecast has informative character and might be used for PV power predictions. On the page is possible to specify starting date and time of the prediction, choose external forecast service from the available (currently `Tomorrow.io <https://www.tomorrow.io/weather/>`_) and select multiple variables to plot. Up to 5 days (adjustable in :doc:`microgrid setup </content/MGsetup>`) of weather forecast are shown in the graph and can be downloaded in csv or json format.

.. image:: /images/forecast_weather.PNG


PV Output Forecast
~~~~~~~~~~~~~~~~~~

Similary, the PV power output is displayed and forecast service can be selected (currently only `meteocontrol <https://www.meteocontrol.com/en/technical-consulting-forecast/forecast/solar-power-forecasting>`_). It is possible to preview PV power predictions per each panel group and in total.

.. image:: /images/forecast_PV.PNG

PV Forecast Validation
~~~~~~~~~~~~~~~~~~~~~~

Here is evaluated precision of the forecasts. Historical predictions are compared with real measured values. Relative and absolute error is calcuated for both, the weather-based and PV forecast. Averaged 15-min data are plotted together in the graph.

.. image:: /images/forecast_compare.PNG

.. _load-forecast:

Local Load Forecast
~~~~~~~~~~~~~~~~~~~

Load power demand prediction are based on historical data and the model is updated regulary with the most recent measurements. Model is created using `Prophet <https://facebook.github.io/prophet/>`_ library, suitable for time series forecasting with seasonal effects. Prophet's additive regression algoritm takes trends, seasonal effects and holidays into the account. The user can change number of days to predict, starting date and sampling time. Results are shown in the polot with the confidence interval.

.. image:: /images/forecast_load.PNG