# Twitter_Sentiment_LSTM
This project uses an LSTM network to predict tweet sentiment to a 72% accuracy.

## Dependencies:
- Keras
- Pandas
- Numpy
- Sklearn
- Wordcloud
- BeautifulSoup
- NLTK
- Tweepy

The project uses an LSTM network to predict sentiment of tweets. The dataset used is include in the repo and consists of 1.6 million tweets. 

### Data:
The original source for this data was found on kaggle --->  https://www.kaggle.com/kazanova/sentiment140

### How to train the model:
Download the dataset from the link above and rename the csv file to tweets.csv, put this file inside a new folder named data which should be in the main project directory and run the preprocessing python file through the CLI to preprocess the tweets for training.

After running this python file through the CLI you should have 2 new csv files containing the preprocessed tweets and the sentiments file. You can now run the sentiment_classifier.py file through the CLI to train the model. This project already comes with the trained model files in case you want to jump straight into prediction of sentiment on new data.

### Conclusion:
So far I have managed to obtain a 72% accuracy with my model. I believe this is due in part to the vast amount of neutral words found in the data, some of which I have removed during preprocessing. During preprocessing I removed unusual characters that were not UTF-8 compliant. 
