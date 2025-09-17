

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

Two models were developed and trained:

1. **Logistic Regression**
2. **Long Short-Term Memory (LSTM)**

Text data was transformed into feature vectors using the `CountVectorizer` class from the *scikit-learn* library. Additionally, the LSTM model was tuned for performance optimization, and results were compared across the models. Model performance was evaluated primarily using **accuracy** as the metric.

## Model Evaluation

* **Logistic Regression:** 99.53% (highest accuracy)
* **LSTM:** 98.48%
* **Tuned LSTM:** 98.46%

### Key Findings:

* Logistic Regression outperformed the deep learning models, achieving the highest accuracy.
* Both the basic and tuned LSTM models delivered comparable results with only slight variations.
* The results highlight that, in some cases, traditional machine learning approaches can be more effective than deep learning models.

### Conclusion:

With an accuracy of **99.53%**, Logistic Regression proved to be the most effective model for fake news detection in this study. Its efficiency in analyzing text-based features allows for quick and precise classification of news articles as real or fake. This makes it a strong candidate for real-time applications, enabling robust content filtering and preserving the integrity of information dissemination.



 






