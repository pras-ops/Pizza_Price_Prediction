# Pizza Price Prediction

This repository contains a project for predicting the prices of pizza based on various parameters such as the number of toppings, diameter, etc. We explore different machine learning models and utilize Auto Machine Learning to achieve accurate predictions. The project timeline consists of the following steps:

## Importing Libraries and DataSet

We import the necessary libraries and read the dataset using pandas.

## Data Analysis

We perform exploratory data analysis to gain insights into the dataset. Visualizations are created to understand the distribution and relationships between different features.

## Feature Engineering

We perform feature engineering tasks such as one-hot encoding to prepare the data for model training.

## Model Building using ML Algorithms

We build machine learning models to predict pizza prices. The models used are XGB Regressor and Support Vector Regressor. We utilize Grid Search CV to find the best parameters for the XGB Regressor.

## XGB Regressor

We use the XGB Regressor model and grid search to find the optimal hyperparameters. The best parameters are obtained, and the model is trained and evaluated on the test set using evaluation metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared score.

## SVR

We train and evaluate a Support Vector Regressor on the same dataset using the same evaluation metrics.

## Auto ML

We employ the EvalML library, an open-source AutoML library, to automate the machine learning pipeline selection process. We split the data into training and testing sets and run AutoML to find the best algorithm and pipeline for our regression problem. We use the R-squared objective to evaluate the models.

## Saving and Loading the Model

We save the best pipeline obtained from AutoML as a pickle file for future use. The model can be loaded and used for making predictions.

## Final Predictions

We use the loaded model to make predictions on the test dataset.

## Report

The findings of the project are as follows:

-   The XGB Regressor model achieved a better performance with lower MAE, RMSE, and higher R-squared score compared to SVR.
-   The AutoML approach helped in identifying the best algorithm and pipeline, resulting in improved performance compared to manually selected models.
-   The final model obtained from AutoML can be used for accurate pizza price predictions.
