# Credit-Card-Fraud-Detection
Predictive Models and a PowerBI dashbaord to detect potential credit card fraud

## The Problem
Contactless payment is on the rise. The adoption rate was acclerated during the pandemic. With the increased use in credit cards this opens up the window to more fraudulent transactions. Due to the sheer amount of transactions companies need a way to detect fraud as soon as it happens.

## The Solution
This is where predictive models can be helpful. By feeding in variables, models can be built to anaylze the features of a transaction and mark it as fraud or not fraud. This allows companies to catch the fraud sooner rather than later because fraud transactions can have a significant impact on the business.

## The Data
The dataset comes from Kaggle - [Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud). 

> The dataset contains transactions made by credit cards in September 2013 by European cardholders.
> This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
> It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

## Steps Taken
1. Load the data and complete Exploratory Data Analysis
2. Ran three models to evaluate which out of three would be the best for predicting credit card fraud. Models I ran:
	* CART Decision Trees
	* Logistic Regression
	* Random Forest
3. Model Assessment - looked at the AUC of each model to determine which model to use in my PowerBI dashboard
4. Created a PowerBI dashboard running the Logistic Regression R script to predict fraud transactions
5. Built visualizations to show metrics of the data and transactions

## Credit Card Fraud Prediction Dashboard
![CCTransaction Metrics](https://github.com/KianaDean/Credit-Card-Fraud-Detection/blob/fc06761b649699883b386ea884c8bbcb5311cee3/images/CCFraudMetrics.PNG)

![CCTransaction Metrics](https://github.com/KianaDean/Credit-Card-Fraud-Detection/blob/fc06761b649699883b386ea884c8bbcb5311cee3/images/CCFraudTransactions.PNG)
