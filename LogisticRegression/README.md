# Riyadh Restaurants ML Project

## Project Overview
This project applies Machine Learning techniques to classify restaurants in Riyadh into two categories:

- Best Restaurant
- Average Restaurant

The project uses the Riyadh Restaurants (20K Records) dataset from Kaggle and applies Logistic Regression for restaurant classification.

---

## Dataset
Dataset Name:
Riyadh Restaurants (20K Records)

Dataset Source:
https://www.kaggle.com/datasets/fahd09/riyadh-restaurants-20k

---

## Features Used
The following features were used for model training:

- price
- likes
- tips
- photos
- ratingSignals

The rating attribute was used only for creating the target variable and was excluded from the input features to avoid data leakage.

---

## Data Cleaning
The preprocessing and cleaning process included:

- Removing duplicated records
- Encoding categorical price values into numerical values
- Converting attributes into numeric format
- Removing invalid and missing values

After cleaning, the final dataset contained 7,294 records.

---

## Target Variable
The target variable is called:

Restaurant_Class

Class labels:
- 1 → Best Restaurant
- 0 → Average Restaurant

The threshold value was determined using the median rating of the dataset to create balanced classes for the classification task.

---

## Machine Learning Model
The project uses:

- Logistic Regression

The dataset was divided into:
- 80% training data
- 20% testing data

Stratified splitting was used to preserve class balance.

---

## Evaluation Metrics
The model was evaluated using:

- Accuracy
- Precision
- Recall
- Confusion Matrix
- Classification Report

---

## Model Performance
The Logistic Regression model achieved:

- Accuracy: 85.7%
- Precision: 91.6%
- Recall: 78.9%

These results indicate strong classification performance for identifying highly-rated restaurants.

---

## Tools and Technologies
- Python
- Google Colab
- Pandas
- Scikit-learn
