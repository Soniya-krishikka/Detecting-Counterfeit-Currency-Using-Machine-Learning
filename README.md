# Detecting-Counterfeit-Currency-Using-Machine-Learning

This repository contains a project for detecting counterfeit currency using a machine learning model. The project involves preprocessing data, training a logistic regression model, and evaluating its performance on fake currency detection.

## Overview

The dataset used in this project contains features extracted from banknotes, which are used to classify them as either genuine or counterfeit. The goal is to build a logistic regression model that can accurately distinguish between genuine and counterfeit banknotes.

## Installation

To run this project, you need Python and several libraries. You can install the required libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage

### Data Exploration

1. **Loading the Data**: The dataset is loaded from a file named `data_banknote_authentication.txt`. The data does not have headers, so column names are assigned during the loading process.

2. **Data Inspection**: Examine the first few rows and check for any missing values.

3. **Visualization**: Use Seaborn to create pair plots and count plots to visualize the relationships between features and the distribution of the target variable.

### Data Processing

1. **Balancing the Dataset**: Address any class imbalance by randomly undersampling the overrepresented class to ensure a balanced dataset.

2. **Data Splitting**: Divide the dataset into training and test sets to evaluate model performance.

3. **Standardization**: Standardize the feature values to ensure that all features contribute equally to the model.

### Model Training

1. **Logistic Regression**: Train a logistic regression model using the balanced and standardized data.

2. **Model Evaluation**: Evaluate the model's performance using accuracy and confusion matrix. The model's accuracy is assessed to determine how well it distinguishes between genuine and counterfeit banknotes.

### Predictions

1. **Model Prediction**: Use the trained model to predict the class of a new banknote and obtain the probabilities of each class.

## Results

The logistic regression model achieved an accuracy of 98.36% on the test set. The model correctly identified genuine banknotes 100% of the time. Predictions for new banknotes can be made by scaling the feature values and passing them through the trained model.

## Conclusion

This project demonstrates how to use logistic regression for detecting counterfeit banknotes. By preprocessing the data, training the model, and evaluating its performance, you can achieve high accuracy in distinguishing between genuine and counterfeit currency.
