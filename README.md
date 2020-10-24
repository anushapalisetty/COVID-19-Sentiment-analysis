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

### NRC Lexicon Analysis

To understand the emotion or opinion of the text,we make use of NRC dictionary which contains a sentiment for the English words. After tokenizing and cleaning the 
text for each word there is a corresponding sentiment attached to it like joy, fear, surprise etc. Figure 5 shows the Sentiments with respect to their counts. 


![nrc](https://user-images.githubusercontent.com/57431137/97067908-b91b9a80-1590-11eb-90b8-8a646a54c6d0.png)


## 3. Tweet Classification:

Once we get the polarity, we classify the tweets Positve as 1, neutral as 0 and negative as 2. We are performing MultiClassification here. Here the feature extraction is implemented using TF-IDF and proceed for modelling. Preprocessing must be implemented before modelling.

### Sampling:
After data preprocessing the next step is Data modelling. To perform data modelling we split the data using Stratified sampling instead of random sampling which take the equal data from each group of the labelled data.We split the dataset into samples of 60:40 where instead of random sampling.

### Naive Bayes :
Naive Bayes are mostly used in natural language processing (NLP) problems.They calculate the probability of each class for a given text and then output the tag with the highest one. 
