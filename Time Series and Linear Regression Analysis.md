# Time Series and Linear Regression Analysis

### Return Forecasting:
* The Yen Futures Settle Prices plot shows an upwards trend long-term. 
* In the short-term, the price seems to be volatile.

### Based on your time series analysis, would you buy the yen now?

* *The model demonstrates a consistently high confidence interval, so we can conclude the GARCH model is a good fit.* 

* *The beta coefficient (0.95) indicates the slight increase in volatility is expected in the long-term, while the alpha coefficient (0.04) suggests a historically stable return on asset; the alpha and beta combined (0.99) suggests the stable volatility of this asset will persist in the long-term.*

### Is the risk of the yen expected to increase or decrease?

* *Based on the upward trend in the forecast plot, the exchange rate risk is expected to increase slightly over the next 5 days.* 

### Based on the model evaluation, would you feel confident in using these models for trading?

#### *Forecasting Returns using an ARMA Model:*
* *The ARMA model is not a good fit, since the p-value (0.422) is greater than the significane level of 0.05.*

* *Therefore, the coefficient of the autoregressive moving average is NOT statistically significant, and should NOT be kept in the model.*

#### *Forecasting Settle Price using an ARIMA Model:*
* *The ARIMA model forecasts that the Japanese Yen will increase in the near term. However, the autoregressive term has a p-value (0.652) that is greater than the significance level of 0.05.*

* *Therefore, the autoregressive term from this model is NOT statistically significant, and should NOT be relied on to forecast Yen futures accurately.*

#### *Volatility Forecasting with GARCH Model:*
* *The GARCH model results in a p-value (0.00171) that is lower than the significance level of 0.05.  Therefore, this model is statistically significant. The model demonstrates a consistently high confidence interval, so we can conclude the GARCH model is a good fit.*

* *Further analysis using the exponentially weighted moving average (EWMA) to determine if investment in this asset is recommended, since the calculations may be diluted by the distant (less relevant) data.*

### Regression Analysis:
* *The out-of-sample RMSE (0.415) is lower than the in-sample RMSE (0.596). A lower RMSE for training data (in-sample RMSE) indicates a good fit, yet this model has a higher in-sample RMSE. In other words, the model performed better on the testing  data (out-of-sample RMSE) which it had never seen before. Therefore, I would NOT recommend using the predictions from this model.
