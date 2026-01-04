# Fake News Detection System

## Project Overview
This project aims to build a machine learning model that can classify news articles as **Fake** or **Real** using Natural Language Processing (NLP) techniques.

## Problem Statement
Fake news spreads misinformation and affects public opinion.  
The goal of this project is to automatically detect fake news articles using machine learning.

## Dataset
The project uses a publicly available dataset containing fake and real news articles.

Source:
https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset

Files used:
- Fake.csv
- True.csv

## Current Progress (Day 1)
- Project repository created
- Dataset downloaded and organized
- Data loading notebook created
- Basic data understanding completed


## Day 2: Labeling and Dataset Merging

In this step, labels were added to distinguish fake and real news articles:
- Fake news → 0
- Real news → 1

Both datasets were then merged into a single DataFrame to prepare the data for supervised learning.  
The combined dataset was shuffled to ensure the model does not learn any ordering bias.


## Day 3: Text Cleaning and Preprocessing

Natural Language Processing (NLP) requires text to be cleaned before modeling.

In this step:
- All text was converted to lowercase
- Unnecessary patterns such as brackets, extra spaces, and special characters were removed
- A reusable text cleaning function was created using regular expressions
- The cleaning function was applied to the dataset to generate a new cleaned text column

This preprocessing step improves model performance by reducing noise in textual data.

## Exploratory Data Analysis (EDA)

- Analyzed distribution of fake and real news articles
- Dataset is nearly balanced between both classes
- Visualized class distribution using Seaborn countplot

## Day 4: Exploratory Data Analysis (EDA)

- Analyzed fake vs real news distribution
- Verified dataset balance
- Visualized class distribution using Seaborn
- Analyzed article length distribution

## Day 5 – Text Vectorization (TF-IDF)

- Handled missing values in cleaned text
- Removed all the rows containing NAN values
- Applied TF-IDF vectorization to convert text into numerical features
- Verified vocabulary contains meaningful words

## Day 6 – Model Training and Evaluation

- Split data into training and testing sets
- Trained Logistic Regression model on TF-IDF features
- Achieved high accuracy on test data
- Evaluated model using classification report and confusion matrix
