# COVID-19-Sentiment-analysis

## Objective:
Performing sentiment analysis on the COVID-19 twitter data analysis and identify the reaction of user if its positive or negative or neutral. 
The sentiment analysis which is part of Natural Language Processing is implemented utilizing Spark Framework.

## Programming Language and Technologies
Python, PySpark, SparkMLlib, SQLContext

## Approach:

## 1.	COVID-19 Data Preprocessing

The raw data available is not suitable to process the Machine Learning algorithm. In order to process the data to modeling we perform some preprocessing technqiques using pyspark libraries like SparkContext, SQLContext, SparkSession, CountVectorizer and more. We also utilize the the packages form the nltk as part of this process. We extract the tweets and perform the preprocess steps using Pyspark:

•	Tokenization
•	Splitting the sentence into words
•	Removing stopwords,
•	Removing punctuations
•	Handling Emoticons
•	Stemming/Lemmatization
•	Getting key phrases

## 2. Data Visualization

###NRC Lexicon Analysis

To understand the emotion or opinion of the text,we make use of NRC dictionary which contains a sentiment for the English words. After tokenizing and cleaning the 
text for each word there is a corresponding sentiment attached to it like joy, fear, surprise etc. Figure 5 shows the Sentiments with respect to their counts. 


 


## 2. Tweet Classification:

Once we get the polarity, we classify the tweets Positve as 1, neutral as 0 and negative as 2. We are performing MultiClassification here. Here the feature extraction is implemented using TF-IDF and proceed for modelling. Preprocessing must be implemented before modelling.
