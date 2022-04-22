# Optimization of Algorithm

To optimize the algorithm and have the best time series forecasting, several factors of
the stock price data have to be taken into consideration. 

From the exploratory analysis, we are able to narrow down the 
number of concept used and time series analysis models.  

# Optimization upon ARIMA

To provide a more accurate prediction of ARIMA, it will require an additional model to overcome
the lack in measuring change in variance.

## Generalized AutoRegressive Conditional Heteroskedasticity (GARCH)

![GARCHModel.png](../Images/GARCHModel.png)

---
# Use of Neural Network



## Long Short-Term Memory (LSTM)

![LSTM.png](../Images/LSTM.png)
LSTM, a chain-like structure with four layers of neural network, each with different functionalities
* Cell state: Information are being stored
* Forget layer: Information will be completed gotten rid of
* Tanh Layer: Checking whether the information should be filtered or stored in cell state  
* Input layer: New information to be updated to the state
* Output layer: The stored information in cell will be filtered and output

The application of LSTM can reduce

### Variate of LSTM
![StackedLSTM.png](../Images/StackedLSTM.PNG)


By stacking LSTM, it is able to make the model deeper, recombining the learned representation from 
prior layers and create new representation at high levels of abstraction. Hence it allow further optimization of the 
Neural Network.

## Utilization of LSTM

---

# Limitation of ARIMA-GARCH

ARIMA-GARCH using one past data of stock price to forecast and predict the stock price movement. However, when an abnormality happens
such as the **2008 market crash** or even the **sudden increase** in **$GME** or **$AMC**, it is unable to react and
predict accordingly.

Therefore, it is very important to include various factors for the prediction of stock price.

## Use of Different Predictor

By analysing the various factors which might affect the stock price prediction, we have come to the conclusion that **News** can be a good predictor
for the stock price.

## News

The reason for using news as a predictor is due to the relationship that the news and the stock price movement can have.

An example of such is the release of company's earnings report with the stock price movement.

![StockPriceFactors.png](../Images/StockPriceFactors.png)

With the release of a company's earning report, it can influence the price of a stock, a strong earning can result
in the stock price moving up and vice versa. Hence, a conclusion have come upon that news has some correlations with the 
fluctuation of price movement.

## Classification

### Metrics for Classification