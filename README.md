# Semantic Analysis on IMDb Movie Reviews
## Aim and scope of the project: 
The project is about applying natural language processing (NLP) techniques for text analytics on IMDb movie reviews dataset. \
The goal is to develop binary sentiment classification models using supervised machine learning methods and compare their accuracy. 
## Problem statement
The problem is to train the machine to understand the sentiment or feeling expressed in the movie review, and classify it as positive or negative. 
## Proposed solution
The proposed solution is to use a sentiment analysis modeling approach that involves data collection and exploration, data preprocessing, feature extraction, vectorization, n-grams, modeling, hyperparameter tuning, and model deployment.
# Data collection 
The data is obtained from [Kaggle]() and consists of 50,000 labelled reviews with two attributes: text and label. The label is either 0 or 1, indicating negative and positive reviews respectively. 
## Data exploration
The data is balanced with a 50:50 ratio of class distribution. \
The data exploration reveals that the text attribute contains HTML tags, non-alphanumeric characters, special characters, and punctuations that need to be removed. \
## Data preprocessing
The data preprocessing steps include normalization with case folding, HTML tags removal, special characters and punctuation removal, stop words removal, POS tagging, and lemmatization based on the POS tag. \
These steps are performed to turn the text into meaningful features for modeling. 
# Feature extraction
The feature extraction methods used are Bag of Words (BoW) model and term frequency-inverse document frequency (TF-IDF) method. \
BoW is a simple and flexible approach to extract features from text based on the occurrence of words. \
TF-IDF is a statistic that measures the importance of a word in the document based on its frequency and inverse document frequency. \
Both BoW and TF-IDF vectorization are performed on unigram and bigram.
## Modeling and hyperparameter tuning
The modeling involves splitting the data into train, test and validation sets, and applying five supervised machine learning models: Multinomial Naïve Bayes, Logistic Regression, Decision Tree, XGBoost and LightGBM. \
Hyperparameter tuning is performed using GridSearchCV to find the best set of parameters for each model. The models are compared and evaluated based on their accuracy score.
## Summary
The results show that the logistic regression model trained using BoW vectorized unigram data of the processed IMDb review data performed the best with the highest accuracy in sentiment analysis compared to other models. 
