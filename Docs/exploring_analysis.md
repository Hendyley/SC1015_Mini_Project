# Exploratory Analysis

## Analysis of Data Type

Before finding the right model and concept to be applied to this project, it is important to 
learn and understand the type of dataset that we have chosen to use. 

Understanding the perks and limitation the type of dataset that we use is 
invaluable as it can narrow down the concept used.

### What is Time Series

Time Series is a sequence of data points that occur in successive order over some
period of time.

It can be decomposed into three factors:

[![TimeSeriesDecomposition.png](../Images/TimeSeriesDecomposition.png)](../Exploratory/MovingAverage.ipynb)

|                      |                        Explanation                         |
|:--------------------:|:----------------------------------------------------------:|
|        Trend         |                 General Movement over time                 |
|       Seasonal       |      Behavior captured in individual seasonal periods      |
|       Residual       |  Everything not captured by trend and seasonal components  | 

## Exploring Concepts

After the preparation of the data, we must first examine the relevant ML concept to manipulate 
the dataset (Time Series). Thus, there were many concepts which we can choose from:

* Classification
* Curve Fitting
* Descriptive Analysis
* Explanative Analysis
* Exploratory Analysis
* Forecast (Primary)
* Intervention Analysis

## The choices used

As our project focuses on stock market and the prediction of the movement, the primary concept that we utilized is
the forecasting concept, with the main focus upon the trend of time series.

Hence, **Moving Average** was chosen as our basis for the rest of the time series analysis model after.  

# General Concept of Moving Average
Using Moving Average we are able to tell the trend in which our dataset is trending towards. As it captures the average change in our data over time.
* An upwards trend shows an upswing in the price
* A downwards trend shows a decline in the price

The ability to identify the trend is important for the data as it gives a rough gauge for the future movement of the stock.
[![MovingAverage.png](../Images/MovingAverage.png)](../Exploratory/MovingAverage.ipynb)

As seen above, it shows the movement of the price, an upwards trend leading to an easier prediction of an increasing stock price.

However, due to its simplicity and the inability to take seasonality and residual into consideration,
it will decrease the accuracy of the prediction. Even with a variating weight, giving more emphasis
on the more recent observation, it is still not very accurate.

|              EMA              |                  Price Movement                   |
|:-----------------------------:|:-------------------------------------------------:|
 | ![EMA.png](../Images/EMA.png) | ![PriceMovement.png](../Images/PriceMovement.png) |

# How did we come to use ARIMA

# Why did we choose ARIMA 
# 

(Nid segue to algorithm optimization --> use of ARIMA + GARCH)
(Best to add some links to [Moving Average Notebook](../Exploratory/MovingAverage.ipynb) & [ARIMAGARCH Notebook](../Analysis/ARIMA-GARCH/ARIMAGARCHPrediction.ipynb))