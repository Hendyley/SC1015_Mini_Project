# Preparation of Data

For the preparation of data required, first we must determine the appropriate dataset that we can use our algorithm upon.

### Requirement for dataset
* Huge Dataset (At least 10 years of data)
* Appropriate sources (Open Source & Well-Trusted)
* Relevant Variables to predict (Adjusted Closing/News) 

Therefore, the dataset that we have <a href="#description">sourced</a> have met the criteria of the dataset.
<div id="top"></div>

## Extracting of Data
How we extract News data
* through HTTP Request through RapidAPI to pull google news
* ![Rapid API](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSjirIYmedE8VAGtlHrscc1nwyZlPNQBQpV8g&usqp=CAU)
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

## Cleaning of Data

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

#### APPLENEWS_Prediction
|  Published Date  |        Date         |           Title           |           Link           |
|:----------------:|:-------------------:|:-------------------------:|:------------------------:|
| Publication Date | Date of the article | Title of the news article | URL for the news article | 

<p align="right">(<a href="#top">back to top</a>)</p>
