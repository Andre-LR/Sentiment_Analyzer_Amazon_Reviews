# Sentiment analyzer with Amazon reviews dataset
[![GitHub license](https://img.shields.io/github/license/Andre-LR/Sentiment_Analyzer_Amazon_Reviews)](https://github.com/Andre-LR/Sentiment_Analyzer_Amazon_Reviews/blob/main/LICENSE)

# About the project
The main goal of this project is to implements classifiers machine learning algorithms to label differents reviews given to amazon products (positive, negative and neutral). The chosen ML algorithms were K-nn, Vader and Logistic Regression.

The project was developed in 5 stages:
  - Dataset reading and analysis
  - Pre-processing with data cleaning
  - Creating training, validation and testing datasets
  - Model classification
  - Results
 
 In order to verify the accuracy of the results obtained, the following evaluation metrics were used:
  - Accuracy
  - Precision
  - Recall
  - F-measure
  
 # Technologies and libraries 
  - Python
  - Jupyter
  - Pandas
  - Matplotlib
  - Scikit-learn (sklearn)
  - Natural Language Toolkit (nltk)


# Step 1. Dataset reading and analysis
First, was checked the score given by the customers to amazon's products. Notice that most of the reviewed, looking to their score, were positive.
| Score | Count |
|-------|-------|
| 1     | 467   |
| 2     | 289   |
| 3     | 395   |
| 4     | 711   |
| 5     | 3131  |

Due to this, the text labeling step was given according to the "Score" of the review.

        Score > 3: Positive

        Score < 3: Negative

        Score = 3: Neutral


# Step 2. Pre-processing with data cleaning
The objective of this step was to remove everything that possible may cause problems to our classification models.

Due to it, we did the following steps:
  - Remove null values
  - Remove duplicate reviews
  - Remove HTML tags 
  - Remove special characters 
  - Put the text reviews to lowercase 
  - Remove stopwords 
  - Data normalization with 'stemming' technique

# Step 3. Training, validation and testing datasets
In order to ensure more reliability in the generated classification models, the dataset was divided into 3 sub-datasets (training, validation and testing) using the “70/10/20” rule. This way, the models won't generate random classification results at each run.

# Step 4. Model classification

## KNN (K Nearest Neighbors)
This classification algorithm tries to predict the correct class for the test data by calculating the distance between the test data and all the training points. Then select the K number of points which is closet to the test data. The KNN algorithm calculates the probability of the test data belonging to the classes of ‘K’ training data and class holds the highest probability will be selected.

## Vader - Valence Aware Dictionary and sEntiment Reasoner
Vader is an open source Python library built for use in sentiment analysis tasks.

Vader works in a very simple way: it has a collection of words, where each word already has a note (or feeling) assigned, and when passed a document (phrase) it returns the following values in percentage:

        pos: how positive is that sentence/document;

        neu: how neutral is the sentence/document;

        neg: how much is negative;

Compound: is the metric used to indicate the final conclusion regarding the sentence as a whole. It is calculated by adding the valence scores of each word in the lexicon, which generates a number between -1 (very negative) and +1 (very positive).

        If compound >= 0.05 -> Positive

        If compound <= -0.05 -> Negative

        If compounding between -0.04 and 0.04 -> Neutral

The compound is the most important metric when you just want to know if that sentence is positive or negative, because its value can be converted into those respective categories and that's exactly what we're going to learn to do here!

## Logistic Regression
Logistic Regression is a probabilistic prediction model that seeks to predict a binary value of 0 or 1, which is more malleable and can be used in complex classification cases. In the formula of this method, outliers are not considered, since they are only considered data close to a line that divides the data according to the specified attributes. Like the Perceptron algorithm, it is an algorithm that requires a lot of training and can only find a linear separator for the data if the data are linearly separable.

# Step 5. Results


# Author

André Luiz Rodrigues

https://www.linkedin.com/in/andreluizzr


