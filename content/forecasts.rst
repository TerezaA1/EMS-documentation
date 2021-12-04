Forecasts
=========

The forecasts page shows all necessary predictions. Microgrid's energy management system uses predictive control for optimal operation of the system and must utilize power forecasts. They are also used for Day-Ahead planning.


Weather Forecasts
~~~~~~~~~~~~~~~~~

The weather forecast has an informative character and might be used for PV power predictions. On the page is possible to specify the starting date and time of the prediction, choose an external forecast service from the available (currently `Tomorrow.io <https://www.tomorrow.io/weather/>`_) and select multiple variables to plot. Up to 5 days of weather forecast are shown in the graph and can be downloaded in CSV or JSON format.

.. image:: /images/ver02/forecast_weather.PNG

|


PV Output Forecast
~~~~~~~~~~~~~~~~~~

Similarly, the PV power output is displayed and forecast service can be selected (external `Solcast <https://solcast.com/>`_ or internal AMOS forecast).

.. image:: /images/forecast_PV.PNG

|


PV Forecast Validation
~~~~~~~~~~~~~~~~~~~~~~

The precision of the forecasts is evaluated, historical predictions are compared with real measured values. Relative and absolute error is calculated for all available methods. Averaged 15-min data and deviation errors are plotted in the graphs.

.. image:: /images/ver02/forecast_compare.PNG

|

.. _load-forecast:

Local Load Forecast
~~~~~~~~~~~~~~~~~~~

Load power demand predictions are based on historical data and the model is updated regularly with the most recent measurements. Model is created using `Prophet <https://facebook.github.io/prophet/>`_ library, suitable for time series forecasting with seasonal effects. Prophet's additive regression algorithm takes trends, seasonal effects and holidays into account. The user can change the number of days to predict, starting date and sampling time. Results are shown in the plot with the confidence interval.

.. image:: /images/forecast_load.PNG

|
