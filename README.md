## Movie Review Sentiment Analysis with SVM

This project predicts the sentiment (positive or negative) of a single sentence from a review of a movie, restaurant, or product.

## Data

The data set consists of 3000 labeled sentences, which are split into a training set of size 2500 and a test set of size 500.

## Preprocessing

The data is preprocessed by:

* Removing leading and trailing white space
* Separating the sentences from the labels
* Transforming the labels from '0 versus 1' to '-1 versus 1'
* Removing digits
* Removing punctuation
* Converting all text to lowercase
* Removing stop words
* Feature Extraction

The data is transformed into a bag-of-words representation using CountVectorizer.

## Classification

A support vector machine (SVM) is used to classify the sentiment of the sentences. The hyperparameter C is tuned to find the best performance.

## Results

The best test error is achieved with C = 1.0.

## Files

`sentiment_analysis.py`: Contains the code for data loading, preprocessing, feature extraction, classification, and evaluation.

## Requirements

* numpy
* matplotlib
* sklearn
  
## How to Run

* Save the code as sentiment_analysis.py
* Install the required libraries (numpy, matplotlib, scikit-learn)
* Run the script: python sentiment_analysis.py
* This will print the training and test error for different values of the C hyperparameter.
