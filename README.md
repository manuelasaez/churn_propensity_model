# Customer Churn Prediction

This repository contains a machine learning project for predicting customer churn in a bank dataset. The goal is to identify customers who are likely to leave the service, enabling the business to take proactive steps to retain them.

## Project Structure

- `train_df.csv`: Training dataset with features about customers and a target column indicating churn (1 for churn, 0 for not churn).
- `test_df.csv`: Test dataset with customer features for which we will predict churn probabilities.
- `notebooks/`: Jupyter notebooks with data exploration, feature engineering, model training, and evaluation steps.
- `src/`: Python scripts used for data processing, model training, and prediction.

## Features

The dataset includes the following features:

- `CustomerID`: Unique identifier for each customer
- `Surname`: Customer's surname (not used in the model)
- `CreditScore`: Customer's credit score
- `Geography`: Country where the customer resides (France, Spain, Germany)
- `Gender`: Customer's gender
- `Age`: Customer's age
- `Tenure`: Number of years the customer has been with the bank
- `Balance`: Customer's account balance
- `NumOfProducts`: Number of bank products the customer uses
- `HasCrCard`: Whether the customer has a credit card (1 for yes, 0 for no)
- `IsActiveMember`: Whether the customer is an active member (1 for yes, 0 for no)
- `EstimatedSalary`: Estimated salary of the customer
- `Exited`: Target variable (1 if the customer has churned, 0 otherwise)

## Project Workflow

1. **Data Exploration**: Initial data analysis, handling missing values, and visualizing the distribution of features.
2. **Data Preprocessing**: Encoding categorical variables, scaling numerical features, and handling imbalanced classes.
3. **Feature Selection**: Using recursive feature elimination to select the most predictive features.
4. **Model Training**: Training a `RandomForestClassifier` model with class weights to handle the imbalance in the target variable.
5. **Model Evaluation**: Evaluating the model using metrics like accuracy, F1-score, recall, precision, and ROC-AUC to determine performance.
6. **Prediction on Test Data**: Making predictions on the test dataset and saving results.


