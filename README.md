About
========================
[![Bull vs Bear][project-screenshot]](https://www.captiveinternational.com/media/image/shutterstock_1695151366_na_studio.jpg)

With the abundance of trading platform such as [MooMoo](https://www.moomoo.com/sg/) and [Tiger broker](https://www.tigerbrokers.com.sg/), stock market 
has been increasingly attractive to consumers. Hence, the stock market has become an interest of many, including us.

Therefore, this project aims to predict future movement of a stock by analyzing history of the stock.

We have chosen Apple stock (**AAPL**) as a sample to test our method for analyzing and 
predicting the movement of the market. 

<div id="top"></div>

## Goal and Requirement
### Goal
Our goal is to predict stock price movement by using machine learning (**ML**) concepts.
To analyze the best concept to predict the movement of stock and test 
the accuracy of the model. 
### Criteria
In order to attain our goal, these criteria have to be met first.
* Select suitable variables to predict the movement of the stock price.
* Select suitable ML concepts to best predict the movement. 
  1. Linear Model
  2. Classification
  3. Neural Network
* Compare and test the accuracy of the model

### Key Learning
 * Linear Model
  * AutoRegressive Integration Moving Average & Generalized AutoRegressive Conditional Heteroskedasticity (ARIMA-GARCH) Model
* Classification
  * Decision Tree Model
* Neural Network
  * Recurring Neural Network (RNN)
    * Long Short Term Memory (LSTM)
  * Natural Language Processing (NLP)    
<p align="right">(<a href="#top">back to top</a>)</p>

## Procedures
Here are the documentation for the procedures for our project.
1. [Data Preparation](Docs/data_prep.md)
2. [Exploratory Anaylsis](Docs/exploring_analysis.md)
3. [Analytic Visualization](Docs/visual.md)
4. [Algorithmic Optimization](Docs/algo_opt.md)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

In order to run this project, there are several prerequisites to be installed.

### Prerequisites

Installation of Python,pip and Jupyter have to be done. 
Download [python version &gt;3.8 ](https://www.python.org/downloads/)

1. Verify that python is installed properly into your computer.
    ```sh
    py --version
    ```
2. Next, check the status of pip. Skip to step 4 if your version of pip is newest.
   ```sh
   py -m pip --version
   ```
3. To upgrade your pip, run this command.
   ```sh
   py -m pip install --upgrade pip setluptools wheel
   ```
4. Install Jupyter Notebook with:
   ```sh
   pip install notebook
   ```
If faced any error, refer to [Troubleshooting documents for PIP & Python](https://packaging.python.org/en/latest/tutorials/installing-packages/)

### Installation

1. Clone the repo
   ```sh
   git clone Hendyley/SC1015_Mini_Project.git
   ```
2. Run this project in your Jupyter Notebook
   ```sh
   jupyter notebook
   ```

If faced any error, refer to [Troubleshooting Documentation for Jupyter](https://jupyter-notebook.readthedocs.io/en/stable/troubleshooting.html)
<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

These sources are used for the research of this project.

* [Complete Guide to Time-Series Analysis](https://towardsdatascience.com/the-complete-guide-to-time-series-analysis-and-forecasting-70d476bfe775?gi=81cbcf49cf28)
* [Guide for ARIMA forecasting](https://towardsdatascience.com/machine-learning-part-19-time-series-and-autoregressive-integrated-moving-average-model-arima-c1005347b0d7)
* [Research for ARIMA-GARCH model for Stock Price Prediction](https://www.e3s-conferences.org/articles/e3sconf/pdf/2021/68/e3sconf_netid21_02030.pdf)
* [What is ARCH and GARCH model?](https://machinelearningmastery.com/develop-arch-and-garch-models-for-time-series-forecasting-in-python/)
* [Stock Prediction for LSTM](https://www.datacamp.com/community/tutorials/lstm-python-stock-market)
* [Introduction to LSTM](https://machinelearningmastery.com/gentle-introduction-long-short-term-memory-networks-experts/)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[project-screenshot]: https://www.captiveinternational.com/media/image/shutterstock_1695151366_na_studio.jpg
