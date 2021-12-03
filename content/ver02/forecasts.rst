Forecasts
=========

The forecasts page shows all necessary predictions. Microgrid's energy managment system uses predictive control for optimal operation of the system and must utilize power forecasts. They are also used for Day-Ahead planning.


Weather Forecasts
~~~~~~~~~~~~~~~~~

Weather forecast has informative character and might be used for PV power predictions. On the page is possible to specify starting date and time of the prediction, choose external forecast service from the available (currently `Tomorrow.io <https://www.tomorrow.io/weather/>`_) and select multiple variables to plot. Up to 5 days of weather forecast are shown in the graph and can be downloaded in csv or json format.

.. image:: /images/ver02/forecast_weather.PNG


PV Output Forecast
~~~~~~~~~~~~~~~~~~

Similary, the PV power output is displayed and forecast service can be selected (external `Solcast <https://solcast.com/>`_ or internal AMOS forecast).

.. image:: /images/forecast_PV.PNG


PV Forecast Validation
~~~~~~~~~~~~~~~~~~~~~~

Precision of the forecasts is evaluated, historical predictions are compared with real measured values. Relative and absolute error is calcuated for all available methods. Averaged 15-min data and deviation errors are plotted in the graphs.

.. image:: /images/ver02/forecast_compare.PNG

.. _load-forecast:

Local Load Forecast
~~~~~~~~~~~~~~~~~~~

Load power demand prediction are based on historical data and the model is updated regulary with the most recent measurements. Model is created using `Prophet <https://facebook.github.io/prophet/>`_ library, suitable for time series forecasting with seasonal effects. Prophet's additive regression algoritm takes trends, seasonal effects and holidays into the account. The user can change number of days to predict, starting date and sampling time. Results are shown in the polot with the confidence interval.

.. image:: /images/forecast_load.PNG