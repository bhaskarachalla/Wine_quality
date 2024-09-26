# Wine Quality Prediction

This repository contains a project focused on predicting the quality of wine using various machine learning models. The dataset used for this project is based on the quality ratings of red and white wines, where the quality is scored on a scale from 0 to 10.

## Table of Contents
- [Overview](#overview)
- [Data Preprocessing](#data-preprocessing)
- [Outlier Treatment](#outlier-treatment)
- [Models Used](#models-used)
- [Results](#results)

## Overview

Wine quality prediction is a multi-class classification problem where the goal is to accurately predict the quality of wine based on various physicochemical properties. This project utilizes several models to evaluate performance and find the best approach for the prediction task.

## Data Preprocessing

The initial step in this project involves data preprocessing, which includes:
- Loading the dataset from the CSV file.
- Handling missing values, if any.
- Standardizing the features to ensure all input variables contribute equally to the model training.

### Features
The features used for prediction include:
- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol

The target variable is the quality of the wine, which is a categorical variable.

## Outlier Treatment

In this project, outliers are identified but not corrected. The rationale for this approach is that outliers can carry significant information that may enhance the model's learning. Removing outliers could result in a loss of valuable data, especially in a limited dataset. The models are designed to learn from the inherent variability in the data, including the outliers.

However, it is important to note that further exploration and analysis may be warranted to determine the impact of outliers on model performance. In future iterations, techniques such as transformation, capping, or robust scaling could be employed to evaluate their effect on predictive accuracy.

## Models Used

The following models were implemented to predict the quality of the wine:

1. **Random Forest Classifier**
   - A powerful ensemble learning method that combines multiple decision trees to improve classification accuracy and control overfitting.

2. **Neural Network**
   - A feedforward neural network model constructed using PyTorch. The architecture includes multiple layers with ReLU activations, designed to capture complex patterns in the data.

Each model was evaluated using metrics such as accuracy, recall, and a detailed classification report to understand their performance comprehensively.

## Results

The results section provides insights into the performance of each model, showcasing accuracy and other relevant metrics. Detailed classification reports allow for an understanding of how each model performed across different wine quality classes.


