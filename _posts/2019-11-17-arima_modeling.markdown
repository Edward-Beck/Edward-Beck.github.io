---
layout: post
title:      "ARIMA modeling "
date:       2019-11-18 02:00:09 +0000
permalink:  arima_modeling
---


ARIMA modeling 
When tasked with predicting the movement of a time series on of the available functions is the ARIMA model and it only makes sense to start at the beginning so let’s dive into the first to letters. Autoregressive or AR is a combination of weights in a linear equation that flesh out the movement of the time series. The variables of the autoregression are periods of the number of increments that the time series is divided into, differencing which is the process of altering the time series until there is a mean and equal variance throughout. Differencing is determining a root equation, if such an equation is found the time series is said to be stationary. The last variable in autoregression is the error associated with lag and autocorrelation. If there is a positive autocorrelation at the first lag the ARIMA model uses autoregression but if there is a negative autocorrelation at lag one the time series is based upon the moving average or MA.  When a negative autocorrelation exists there are continuous irregularities for multiple consecutive periods. 
The Intergrated component is the difference between the predicted errors of the weighted lags and the actual sum of the weighted lag values…why a hyphen wasn’t used because it really fits well like the Auto-Regressive - Moving Average is beyond my comprehension. 
