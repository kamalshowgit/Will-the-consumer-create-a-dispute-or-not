# Random Forest Classifier for Consumer Complaint Prediction

This repository contains code that demonstrates the use of a Random Forest classifier to predict whether consumer complaints will result in a dispute. The code preprocesses the data, engineers features, trains the classifier, and generates a submission file.

## Table of Contents

- [Introduction](#introduction)
- [Data](#data)
- [Feature Engineering](#feature-engineering)
- [Model Training](#model-training)
- [Predictions and Submission](#predictions-and-submission)
- [Understand Random Forest in 8 Minutes](#understand-random-forest-in-8-minutes)

## Introduction

This code aims to solve a classification task using a Random Forest algorithm. The goal is to predict whether consumer complaints will result in a dispute based on various features.

## Data

The dataset consists of consumer complaints, and the code processes both training and test data. The key steps for data preprocessing include:
- Loading the data from CSV files.
- Converting date columns to datetime format.
- Calculating the time difference between receipt and company response.

## Feature Engineering

The data preprocessing involves several important steps:
- Creating binary columns to indicate missing values in categorical variables.
- Dropping original categorical columns with missing values.
- Encoding the target variable "Consumer disputed?" to binary (1 for "Yes," 0 for "No").
- Creating binary variables for common categories in the "Issue" column.
- Creating binary variables for top states in the "State" column.
- Applying one-hot encoding to categorical variables.

## Model Training

The Random Forest classifier is used for training. Key steps in this section include:
- Importing the necessary libraries and initializing the classifier.
- Preparing the feature matrix and target vector.
- Training the classifier using the `fit` method.

## Predictions and Submission

The trained classifier is used to make predictions on the test data. Steps include:
- Predicting consumer dispute outcomes for the test dataset.
- Converting numeric predictions to "Yes" or "No" labels.
- Creating a submission DataFrame containing "Complaint ID" and predicted values.
- Saving the submission DataFrame to a CSV file named "submission.csv."

## Understand Random Forest in 8 Minutes

For a quick overview of how Random Forest works, you can watch this [video](https://youtu.be/v6VJ2RO66Ag) that explains the concept of Random Forest in just 8 minutes.

This repository serves as an example of how to preprocess text data, engineer relevant features, and utilize a Random Forest classifier for a classification task.
