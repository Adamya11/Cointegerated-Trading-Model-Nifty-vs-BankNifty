# Cointegerated-Trading-Model-Nifty-vs-BankNifty

In financial markets and in the real world, there are time series which are cointegrated. In general terms if two time series are ‘cointegrated’ then it means, that the two time-series move together and if at all there is a deviation from this movement, it is either temporary or can be attributed to a stray event, and one can expect the two time-series to revert to its regular orbit i.e. converge and move together again. This type of time series is exactly what we want to find in financial markets.

So, in this project I will try and find this cointegrated relationship between Nifty Index and Bank Nifty Index.

To find a cointegrated time series we will try different regression techniques and select the most accurate technique which works on our data. Regression in basic terms comes with the relationship between Independent variable X and dependent variable Y. That relationship is described in terms of slope. so, slope captures how much Y would change with change in X.

Once we get a relationship then we will use that relationship to predict the value of Y from X. But more often regression techniques has a hard time predicting dependent variables properly. so, we are not going to use regression predictions to directly make trades.

Instead of focusing on predictions from the regression model we will going to focus on errors made by the model, also known as residuals. We will check whether the residuals of a model are stationary, the mean and variance of residuals is in tight range and autocorrelation of residuals is close to 0. This means a residual time series is stationary.

Stationarity of residuals confirms that two stocks are cointegrated. They move closely together and if at all some deviation happens that's temporary, they will converge back. 

We will make trades based on Adfuller test results and with the help of some manual features. We will set trigger prices, targets, stoploss and square-off's.
Finally we will check the results of our model by checking the Profits made by our trades on test data.
