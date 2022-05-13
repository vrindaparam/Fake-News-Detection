# Fake-News-Detection
Fake News Detection using Machine learning. 

**Problem Statement:**
The purpose is to identify if a news is Fake or not.

**Overview**
The topic of fake news detection on social media has recently attracted tremendous attention. 
Our project aims to use **Natural Language Processing** to detect fake news directly, based on the text content of news articles.


I've tried to develop a machine learning program to identify when a news source may be producing fake news.
Aim is to use a corpus of labeled real and fake new articles to build a classifier that can make decisions about information 
based on the content from the corpus. 
The model will focus on identifying fake news sources, based on multiple articles originating from a source.
Once a source is labeled as a producer of fake news, we can predict with high confidence that any future articles 
from that source will also be fake news. Focusing on sources widens our article misclassification tolerance, 
because we will have multiple data points coming from each source.

The intended application of the project is for use in applying visibility weights in social media. 
Using weights produced by this model, social networks can make stories which are highly likely to be fake news less visible.

**Approach**
The dataset has 5 columns. 
id: unique id for a news article
title: the title of a news article
author: author of the news article
text: the text of the article; could be incomplete
label: a label that marks the article as potentially unreliable
1: False News or Unreliable
0: True News or reliable

We consider only the text column to train the model.
Natural language processing has been used to remove stopwords. 
Feature Extraction methods CountVectorizer and Tf-IDF Vectorizer have been tried with different Machine learning models.
Machine learning models Passive Aggresive Classifier gave 99.29 accuracy and Mulitnomial Naive  Bayes with 93.56% accuracy.
Confussion Matrix and accuracy was chosen as the metrics to evaluate the best model . 


