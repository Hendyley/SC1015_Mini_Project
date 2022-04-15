# Preparation of Data

For the preparation of data required, first we must determine the appropriate dataset that we can use our algorithm upon.

### Requirement for dataset
* Huge Dataset (At least 10 years of data)
* Appropriate sources (Open Source & Well-Trusted)
* Relevant Variables to predict (Adjusted Closing/News)
* Able to fit within the algorithm utilized (LSTM/ARIMA-GARCH/Classification)

Therefore, the dataset that we have <a href="#description">sourced</a> have met the criteria of the dataset.
<div id="top"></div>

## Extracting of Data

### News Data
The extraction of news data is:
* through HTTP Request through RapidAPI to pull google news

![Rapid API](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSjirIYmedE8VAGtlHrscc1nwyZlPNQBQpV8g&usqp=CAU)

The implementation of the extraction of data
```python
url = "https://google-news1.p.rapidapi.com/search"

querystring = {"q":"Apple","country":"US","lang":"en","before":"2021-10-10","after":"2021-09-08"}

headers = {
	"X-RapidAPI-Host": "google-news1.p.rapidapi.com",
	"X-RapidAPI-Key": "60ba6c2c8emsha8a15e53ec84acdp14aeb3jsncd684f9e15bd"
}

response = requests.request("GET", url, headers=headers, params=querystring)
x = response.text
```

The output will be in Json Format.

But we can change it to dataframe format.

```python
data = json.loads(x)
News_Test = pd.json_normalize(data["articles"])
#News_Test.head()
```
### Stock Price Data

The extraction of the 40 years worth of data is pulled through Kaggle, and exported to an Excel sheet.

<p align="right">(<a href="#top">back to top</a>)</p>

## Cleaning of Data

### News Data

### Stock Price Data

Due to the first 30 years having little fluctuation as compared to the recent years, 
the training dataset has been cleaned to only include the more recent years.
Hence, the dataset spans only the past decade, from 2013 to 2021.

<p align="right">(<a href="#top">back to top</a>)</p>

## Appendix
### Sources & Tools Used to Extract Data
* [Kaggle](https://www.kaggle.com/datasets/meetnagadia/apple-stock-price-from-19802021/code)
* [Rapid API](https://rapidapi.com/newscatcher-api-newscatcher-api-default/api/google-news)
* [Yahoo Finance API](https://pandas-datareader.readthedocs.io/en/latest/)

### Description of Datasets
<div id="description"></div>

#### APPLTrain.csv/APPLTest.csv
|           Date           |           Open           |           High           |           Low           |          Close           |                          Adj Closing                           |            Volume            |
|:------------------------:|:------------------------:|:------------------------:|:-----------------------:|:------------------------:|:--------------------------------------------------------------:|:----------------------------:|
| Date of the stock market | Opening Price of the day | Highest Price of the day | Lowest Price of the day | Closing Price of the day | Adjusted Price for closing. (Used when there is a stock split) | Total Volume bought and sold |

#### APPLNEWS_Train.csv/APPLNEWS_Test.csv
|  Published Date  |        Date         |           Title           |           Link           |
|:----------------:|:-------------------:|:-------------------------:|:------------------------:|
| Publication Date | Date of the article | Title of the news article | URL for the news article | 

<p align="right">(<a href="#top">back to top</a>)</p>
