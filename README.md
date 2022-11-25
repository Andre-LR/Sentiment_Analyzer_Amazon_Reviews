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

# Step 3. Creating training, validation and testing datasets

# Step 4. Model classification

# Step 5. Results


# Author

André Luiz Rodrigues

https://www.linkedin.com/in/andreluizzr


