

# **Fake News Detection**


## Authors

Arshpreet Kaur


## Introduction

In today’s digital era, the rapid spread of misinformation—commonly referred to as fake news—has emerged as a serious global challenge. It undermines the credibility of journalistic institutions and disrupts informed decision-making across societies. Beyond politics, fake news has had significant consequences in areas such as public health. During the COVID-19 pandemic, misinformation triggered panic-buying of unverified remedies and fueled vaccine hesitancy, hampering efforts to control the virus. Tackling this problem requires data-driven approaches that leverage machine learning, natural language processing, and social network analysis. Researchers and policymakers are increasingly employing these methods to detect and curb misinformation, enabling more targeted interventions to mitigate its harmful effects.

## Problem Statement

The central issue addressed in this study is the widespread presence of fake news in digital media. Its dissemination erodes public trust, damages the credibility of news organizations, and polarizes societies. Moreover, unchecked misinformation can escalate into broader consequences such as social unrest, political instability, and even legal challenges.

## Main Objective

* To design and implement robust fake news detection mechanisms that can identify and flag misinformation in real time, thereby safeguarding the integrity and credibility of the news ecosystem.

## Data Understanding

The dataset for this project was sourced from [Kaggle](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset). It consists of two files:

* **Fake.csv** → 23,481 rows and 4 columns
* **True.csv** → 21,417 rows and 4 columns

## Data Preparation

Data preprocessing involved several steps to ensure quality and consistency:

* Cleaning and handling missing values
* Removing duplicates
* Performing Exploratory Data Analysis (EDA) to uncover patterns, distributions, and correlations—informing model selection and hyperparameter tuning

For text preprocessing, the following steps were carried out:

* Lowercasing all text
* Removing punctuation, digits, and stop words
* Applying stemming or lemmatization to reduce words to their root forms

These steps streamlined the text data, reducing noise and complexity while focusing on essential linguistic features for effective model training.

## Modeling

Four models were developed and trained:

1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Gradient Boosting Classifier**
4. **Random Forest Classifier**


## Model Evaluation

* **Logistic Regression:** 98.59% 
* **DT Classifier:** 99.58%
* **GB Classifier:** 99.52%
* **RF Classifier:** 98.65%

### Key Findings:

* High Performance Overall: All four models performed exceptionally well, with accuracy scores ranging from 98.59% to 99.58%. This indicates that the dataset is well-suited for a standard machine learning approach and that the features you used (likely the TF-IDF vectorized text) are highly effective at distinguishing between fake and true news.

* Decision Tree Classifier is the Top Performer: The Decision Tree (DT) Classifier achieved the highest accuracy at 99.58%, making it the best-performing model among the four.

* Gradient Boosting is a Close Second: The Gradient Boosting (GB) Classifier was a very close second with an accuracy of 99.52%, nearly matching the performance of the Decision Tree.

* Similar Performance from Logistic Regression and Random Forest: The Logistic Regression and Random Forest (RF) Classifier models showed very similar performance to each other, with scores of 98.59% and 98.65% respectively. While still excellent, they are slightly less accurate than the top two models.

### Conclusion:

The primary conclusion is that a simple Decision Tree Classifier is the most effective model for this particular fake news detection problem, providing the highest accuracy with a very straightforward implementation. Both the Decision Tree and Gradient Boosting models demonstrate a near-perfect ability to classify news articles as fake or true.

The high accuracy of all models suggests that the problem is not particularly complex, and even basic models like Logistic Regression can achieve strong results. For a production environment, the Decision Tree would be a great choice due to its high accuracy and often faster prediction speed compared to more complex ensemble models like Gradient Boosting.



 






