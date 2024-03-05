# Abstract
This project is to predict sum of other parties' bet at time we bet so that we can get the most dividends.
We can see that the horse racing data is irregularly-spaced time series. Therefore, to easily build a time series model, we have to transform the data into a regularly-spaced format. The data will be a monthly time series. Then I used STL (Seasonal and Trend decomposition using Loess) to decompose the time series data to check the trend and seasonality.
After observing the ACF and PACF plot, find the appropriate argument for ARIMA model, then fit the model. The final MSE on test set is 0.3358 after normalization.
Used (past bets, number of races every day, true winning probability of horses) as input feature sequences, and feed them into LSTM model. Decreases MSE 15% lower.
