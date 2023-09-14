# Fraud-Detect-Transaction

## 1. Introduction 

Source Kaggle.com; data provided by Vesta
Shape (size) : 590540 records, 433 features
More info (https://www.kaggle.com/c/ieee-fraud-detection/data)
Problem: binary classification

Code:https://github.com/aabdygaziev/capstone-project

Challenges: Large dataset, a lot of missing values, imbalanced data and feature selection.\

![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/780e3ee8-5f45-4cbe-9ff1-2aa0e73e9d53)

## 1. Fraud Transactions Dataset
The fraud transactions dataset contains information on a series of transactions, including the transaction date and time, credit card number, merchant, and transaction category. This report will provide an overview of the dataset and its columns, including the data types, number of unique values, and other statistical information.

This dataset is fictional and is trying to simulate real life details. Any similarity to real life cases is purely coincidental.
It has the following columns.

trans_date_trans_time: The date and time of the transaction.

cc_num: credit card number.

merchant: Merchant who was getting paid.

category: In what area does that merchant deal.

amt: Amount of money in American Dollars.

first: first name of the card holder.

last: last name of the card holder.

gender: Gender of the cardholder.Just male and female!

street:Street of card holder residence

city:city of card holder residence

state:state of card holder residence

zip:ZIP code of card holder residence

lat:latitude of card holder

long:longitude of card holder

city_pop:Population of the city

job:trade of the card holder

dob:Date of birth of the card holder

trans_num: Transaction ID

unix_time: Unix time which is the time calculated since 1970 to today.

merch_lat: latitude of the merchant

merch_long:longitude of the merchant

is_fraud: Whether the transaction is fraud(1) or not(0)
