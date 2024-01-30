# Credit Card Fraud Detection

## Project/Goals
Overview:

The primary objective of the project is to gain insights into credit card fraud through exploratory data analysis, which includes creating visualizations and dashboards to observe and identify trends in various aspects. This involves:

1. Analyzing the distribution of transaction amounts between fraudulent and legitimate transactions.
2. Examining transactions based on the time of day.
3. Identifying geographical patterns of transactions.
4. Investigating the correlation between certain variables and the occurrence of fraud.
5. Assessing whether specific merchants are more susceptible to fraud than others.
6. Exploring activities of individuals who are noticeable for fraudulent activities, including analyzing their Date of Birth (DOB), job information, and genders.

Additionally, a secondary objective is to explore and develop a regression model based on the available dataset.

## About the Dataset
### Description

This dataset simulates credit card transactions, encompassing both legitimate and fraudulent activities, spanning from January 1, 2019, to December 31, 2020. It involves transactions conducted by 1000 customers with a diverse pool of 800 merchants.

Transactions are classified into 14 different categories, with only 9651 out of the 1.85 million transactions (0.52%) were identified as fraudulent.

### Dataset Link
[Credit Card Fraud Dataset on Kaggle](https://www.kaggle.com/datasets/kartik2112/fraud-detection)

### Columns available in Dataset
    Timestamps: Both trans_date_trans_time and unix_time allowing for time-based pattern analysis.

    Merchant Details: Includes the name of the merchant and geolocations (latitude & longitude).

    Transaction Details: Indicates the category of the purchased product and the amount of the transactions.

    Credit Card Holder Information: Encompasses names, gender, dates of birth, addresses, geolocations and credit card numbers.

    Fraud Indicator (is_fraud): 1 for fraudulent transactions, 0 for legitimate transactions.

## Process
### Data Prep

1. Imported two CSV files and check for columns name and see if two data file can be merged together.
2. Upon checking the columns name and type matches, proceed with merge two data file into one dataframe.
3. Delete index column and export to CSV file for further processing.

## Results

## Challenges 


## Future Goals

