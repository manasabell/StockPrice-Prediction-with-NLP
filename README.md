# ISM-6930-Data-Science-Project
Stock Price Market Movement using News Headlines

Data from https://www.kaggle.com/aaron7sun/stocknews

In this project, we are trying to predict the DOW Jones stock market movement based on the sentiment values extracted from the Top Headlines scrapped from the Reddit Website using the API. 

'''

Setup Info

conda create -n news_stock python=3.7 anaconda

activate news_stock

pip install xgboost
pip install nltk


Data Info :

Added sentiment values to csv using jupyter notebook "Extracting Sentiment from News Headlines.ipynb" and saving to "combined with sentiment.csv" CSV File.

Added "Start trend" column by comparing current days opening value with previous days adjecent close value and saved it to "Combined_News_DJIA_with_start.csv" CSV File.

Two Jupyter notebooks:

1. predict stock market movement with sentiment values and start trend.ipynb - In this code, we have considered the compound values of sentiments from top 25 news headlines for each date and the "Start trend" value which is a binary value with 1 = upward trend and 0 = downward trend

2.Predicting Stock Movement with Sentiment and Stock values.ipynb = In this code, we have considered all the stock market values like Open value, Close value, Low, High, Volume, Adjacent Close value and Start trend as well as the Compound value of sentiment from news headlines.

To run these Jupyter notebooks, all the csv files and the notebooks should be placed in the same folder.


Credits :

Sun, J. (2016, August). Daily News for Stock Market Prediction, Version 1. Retrieved 03/25/2019 from https://www.kaggle.com/aaron7sun/stocknews

https://www.kaggle.com/lseiyjg/use-news-to-predict-stock-markets

http://t-redactyl.io/blog/2017/04/using-vader-to-handle-sentiment-analysis-with-social-media-text.html

'''
