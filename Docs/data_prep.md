#Preparation of Data
For the preparation of data required, first we must determine the appropriate dataset that we can use our algorithm upon.
### Requirement for dataset
* Huge Dataset (At least 10 years of data)
* Appropriate sources (Open Source & Well-Trusted)
* Relevant Variables to predict (Adjusted Closing/News)

Therefore, the dataset that we have <a href="#description">sourced</a> have met the criteria of the dataset.
<div id="top"></div>

## Cleaning of Data

<p align="right">(<a href="#top">back to top</a>)</p>

##
<p align="right">(<a href="#top">back to top</a>)</p>

##
<p align="right">(<a href="#top">back to top</a>)</p>

##
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

#### APPLE_NEWS

|          Title           |     Link     |             Keyword              |        Creator         |                 Video URL                  |      Description       |          Content           |       PubDate       |           Full Description           |                 Image URL                 | Source ID |
|:------------------------:|:------------:|:--------------------------------:|:----------------------:|:------------------------------------------:|:----------------------:|:--------------------------:|:-------------------:|:------------------------------------:|:-----------------------------------------:|:---------:|
| Title of the new article | News article | Keywords used within the article | Creator of the article | A URL of any video used within the article | Summary of the article | Description of the content | Date of publication | Full Description of the news article | URL to any images used within the article | Publisher |
###### Deprecated

#### APPLENEWS_Prediction
|  Published Date  |        Date         |           Title           |           Link           |
|:----------------:|:-------------------:|:-------------------------:|:------------------------:|
| Publication Date | Date of the article | Title of the news article | URL for the news article | 

<p align="right">(<a href="#top">back to top</a>)</p>