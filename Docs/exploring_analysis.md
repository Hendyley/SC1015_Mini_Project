# Exploratory Analysis
The Exploratory Analysis would expand upon how we applied the ARIMA and LSTM into our time series model.

# Where did we start (Comparison of variables) (Correlation model)
* Firstly, we need to know whether our model is stationary, as it shows the constancy to the data over time.
  * To do that, we used the Dickey-Fuller Test to determined stationarity.
* Secondly, whether our model had any seasonality.
  * Seasonality refers to a regular and predictable pattern that repeats over the time series data which could negatively affect the regression model.
  * To do that, we used the Autocorrelation Function (ACF) to determined seasonality.
* Once we determined the factors above, we had to find the Moving Average(MA) of our model.
* Next step was to apply differencing in order to make our model stationary.
* <a href="#continue">Continue</a>

# Concept of Moving Average
Using Moving Average we are able to tell the trend in which our dataset is trending towards. As it captures the average change in our data over time.
* An upwards trend shows an upswing in the price
* A downwards trend shows a decline in the price

Therefore, using Moving Average we are able to tell beforehand whether the stock price is trending upwards or downwards which would help in our prediction.

# How did we come to use ARIMA/LSTM
We needed a model which is capable of predicting future values based on past values, and ARIMA is capable of performing that as it makes use of lagged moving averages to smoothen the time series data.

ARIMA uses a set of parameters called p,d,q to make prediction based on the given model. 

p - The number of lag observations in the model.

d - The number of differences needed for stationarity.

q - The number of lagged forecast errors in the prediction equation.

<div id="continue"></div>

* Once the model is stationary, we can train our ARIMA model to find the best sets of parameters to fit into our model.
* Applying the given p,d,q values into the ARIMA function, we are able to predict future values.
* Now, we compare our predicted value against the test value.

# Why did we choose ARIMA and LSTM (Advantages of using them over Moving Average)
# 
