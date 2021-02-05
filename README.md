# Election Sentiment Analysis

This project aims to see the dynamic of U.S. 2020 Election by looking at the sentiment of both candidates through a famous microbloggins social media Twitter. Through this sentiment analysis it is expected to see which candidates is more favorable, and if developed further there is a chance this sentiment analysis could bring accurate prediction of the election. 
<p>&nbsp;</p>

## Scraper
SNScrape is used to scrape tweets, in order to use this scraper the Python Environment must be Python 3.8 or above. Unlike most Twitter scraper (such as Tweepy), SNScrape requires no authentication and it also scrape old tweets. https://github.com/JustAnotherArchivist/snscrape. Keywords for querying tweets are the name of the candidates. Language filter also applied to make sure scraped tweets are in English.
<p>&nbsp;</p>

## Model
The neural network model is built using LSTM. Through LSTM the semantic of a sentence is preserved through words. The model is built on TensorFlow framework. The dataset used for training contains 1,578,000 tweets with its sentiment with 80-20 training-test split ratio. The model is trained for 8 iterations and the model achieved 85.41% accuracy, 0.3342 loss, 83.28% validation accuracy, and 0.3791 validation loss (indicating slight overfitting).

## Sentiment Analysis
Through sentiment analysis, there are more positive sentiments than negative sentiments for both candidates but out of 15,000 tweets Joe Biden receives more positive sentiment compared to Donald Trump. The tweets also visualized in wordcloud, indicating that Joe Biden is more favorable which seen through word 'Win' appear the biggest in Joe Biden's wordcloud.
