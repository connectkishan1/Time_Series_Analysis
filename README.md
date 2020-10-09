# Time_Series_Analysis
Time series analysis is a statistical technique that deals with time series data, or trend analysis.  Time series data means that data is in a series of  particular time periods or intervals.  The data is considered in three types:

Time series data: A set of observations on the values that a variable takes at different times.

Cross-sectional data: Data of one or more variables, collected at the same point in time.

Pooled data: A combination of time series data and cross-sectional data.

## Terms and concepts:

Dependence: Dependence refers to the association of two observations with the same variable, at prior time points.

Stationarity: Shows the mean value of the series that remains constant over a time period; if past effects accumulate and the values increase toward infinity, then stationarity is not met.

Differencing: Used to make the series stationary, to De-trend, and to control the auto-correlations; however, some time series analyses do not require differencing and over-differenced series can produce inaccurate estimates.

Specification: May involve the testing of the linear or non-linear relationships of dependent variables by using models such as ARIMA, ARCH, GARCH, VAR, Co-integration, etc.
ARIMA:

ARIMA stands for autoregressive integrated moving average.  This method is also known as the Box-Jenkins method.

## Identification of ARIMA parameters:

Autoregressive component: AR stands for autoregressive.  Autoregressive paratmeter is denoted by p.  When p =0, it means that there is no auto-correlation in the series.  When p=1, it means that the series auto-correlation is till one lag.

Integrated: In ARIMA time series analysis, integrated is denoted by d.  Integration is the inverse of differencing.  When d=0, it means the series is stationary and we do not need to take the difference of it.  When d=1, it means that the series is not stationary and to make it stationary, we need to take the first difference.  When d=2, it means that the series has been differenced twice.  Usually, more than two time difference is not reliable.

Moving average component: MA stands for moving the average, which is denoted by q.  In ARIMA, moving average q=1 means that it is an error term and there is auto-correlation with one lag.

In order to test whether or not the series and their error term is auto correlated, we usually use W-D test, ACF, and PACF.

Decomposition: Refers to separating a time series into trend, seasonal effects, and remaining variabilityAssumptions:

Stationarity: The first assumption is that the series are stationary.  Essentially, this means that the series are normally distributed and the mean and variance are constant over a long time period.

Uncorrelated random error: We assume that the error term is randomly distributed and the mean and variance are constant over a time period.  The Durbin-Watson test is the standard test for correlated errors.

No outliers: We assume that there is no outlier in the series.  Outliers may affect conclusions strongly and can be misleading
