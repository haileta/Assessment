
Xtern 2024 Artificial Intelligence Data Set Analysis
Project Overview
This project involves analyzing the "Xtern 2024 Artificial Intelligence Data Set" to predict orders. The dataset is initially cleaned, explored, and processed using various data preprocessing techniques. The primary focus is on applying machine learning models to achieve accurate predictions.

Dataset
The dataset is named "Xtern_TrainData.csv" and includes various features relevant to the prediction task. Initial steps include loading the data, handling missing values, and examining data types and the first few entries.

Key Operations
Data Cleaning and Exploration: Missing values are removed, and data types are checked. The head() function is used to view the initial rows of the dataset.
Feature Analysis: Unique values of specific features like 'Order', 'University', etc., are analyzed using set().
Machine Learning Pipeline
Data Preparation:

Splitting features (X) and target (y).
Splitting the dataset into training and testing sets.
Model Training:

A RandomForestRegressor is used for initial model training.
The model's performance is evaluated using the score() method.
Data Encoding and Transformation:

Label encoding is applied to the target variable.
OneHot encoding is applied to categorical features using ColumnTransformer.
Model Training on Transformed Data:

The model is re-trained on transformed data.
Performance is evaluated again using the score() method.
Hyperparameter Tuning Using GridSearchCV:

A parameter grid is defined for the RandomForestRegressor.
GridSearchCV is used to find the best model parameters.
Libraries Used
pandas
sklearn (train_test_split, RandomForestRegressor, OneHotEncoder, ColumnTransformer, LabelEncoder, GridSearchCV)
Results
The final model performance (accuracy score) is evaluated on the test set. The best model obtained from GridSearchCV is also evaluated.

How to Use
To use this code:

Ensure you have the required libraries installed.
Load your dataset in place of "Xtern_TrainData.csv".
Run the Python script to perform data preprocessing, model training, and evaluation.
Note
Adjust file paths and variable names as per your dataset.
Consider customizing the model and preprocessing steps according to the specific characteristics of your dataset.
