# Riyadh Restaurants ML Project

## Project Overview

This project applies Machine Learning techniques to classify restaurants in Riyadh into two categories:

- Highly Rated Restaurant
- Lower Rated Restaurant

The project uses the Riyadh Restaurants (20K Records) dataset from Kaggle and applies a Logistic Regression model for restaurant classification.

---

## Dataset

### Dataset Name
Riyadh Restaurants (20K Records)

### Dataset Source
https://www.kaggle.com/datasets/fahd09/riyadh-restaurants-20k

---

## Features Used

The following features were used for model training:

- price
- likes
- tips
- photos
- ratingSignals

The `rating` attribute was used only for creating the target variable and was excluded from the input features to avoid data leakage.

---

## Data Cleaning

The preprocessing and cleaning process included:

- Removing duplicated records
- Encoding categorical price values into numerical values
- Converting attributes into numeric format
- Removing invalid and missing values

After preprocessing and cleaning, the final dataset contained 7,294 records.

---

## Target Variable

The target variable is called:

`Restaurant_Class`

### Class Labels

- 1 → Highly Rated Restaurant
- 0 → Lower Rated Restaurant

The threshold value was determined using the median rating of the dataset to create balanced classes for the classification task.

Restaurants with ratings greater than or equal to the median rating were classified as Highly Rated Restaurants, while restaurants with ratings below the median rating were classified as Lower Rated Restaurants.

---

## Machine Learning Model

The project uses:

- Logistic Regression

The dataset was divided into:

- 80% training data
- 20% testing data

Stratified splitting was used to preserve class balance between the training and testing datasets.

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
---

## Model Performance

The Decision Tree model achieved:

- Accuracy: 73.5%
- Precision: 73.7%
- Recall: 73.6%

These results indicate balanced classification performance with no overfitting.

---

## Tools and Technologies

- Python
- Google Colab
- Pandas
- Scikit-learn
