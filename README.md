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

- Timestamps: Both trans_date_trans_time and unix_time allowing for time-based pattern analysis.

- Merchant Details: Includes the name of the merchant and geolocations (latitude & longitude).

- Transaction Details: Indicates the category of the purchased product and the amount of the transactions.

- Credit Card Holder Information: Encompasses names, gender, dates of birth, addresses, geolocations and credit card numbers.

- Fraud Indicator (is_fraud): 1 for fraudulent transactions, 0 for legitimate transactions.

## Process
### Data Prep Section

1. Imported two CSV files and check for columns name and see if two data file can be merged together.
2. Upon checking the columns name and type matches, proceed with merge two data file into one dataframe.
3. Delete index column and export to CSV file for further processing.

### EDA

1. Check for null value and duplicate values
2. Calculate the number of total transactions and percentage of fraudulent vs legitimate transactions
3. Removing meaningless columns e.g. Index and Trans_num columns.
4. Update column data types and trim the columns that have prefix which can be removed.
5. Create new column to get full name of credit card holder
6. Create heatmap and correlation matrix based on available dataset.
7. Rearrange the dataframe and export the dataframe to CSV file for further use.

### Regression Model

Initially created regression model based on the available dataset.

The negative R-squared values and unusual F-statistic might indicate issues with the model, we can tell that it might because of imbalance of dataset.

The steps we took next is to resample with sample size 10000 with 50% fraudulent activities and 50% non-fraud activities.

The negative R-squared values, unusual F-statistic, and the fact that many coefficients are very close to zero with high p-values suggest that the model and the individual coefficients are not statistically significant. 

## Results

## Conclusion

Fraudulent transactions exhibited a discernible pattern, predominantly occurring during specific periods, usually a few hours before and after midnight (11PM to 12 AM). 

These fraudulent transactions were distinguished by fairly lower spending amounts. 

While many other transaction patterns mirrored those of legitimate transactions, the scarcity of fraudulent instances in the dataset (i.e., an imbalanced dataset) prevents us from creating a regression model that could offer valuable insights.

