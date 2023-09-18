# Fraud-Detect-Transaction

## I. Introduction 

Source: Kaggle ( [Click here](https://www.kaggle.com/datasets/dermisfit/fraud-transactions-dataset?select=fraudTrain.csv) )

Shape (size) : 2M records, 23 features

Problem: binary classification

**This dataset was already separated into 2 set: train and set dataset**

Code: [Fraud transaction _ Personal Project]([https://colab.research.google.com/drive/1Fq4bxgt6y0bO49D_lR9A9Btprx3mNGbR?usp=sharing])

Challenges: Large dataset, a lot of missing values, imbalanced data and feature selection.

Here is the steps that I'm going to apply for this project: 

![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/780e3ee8-5f45-4cbe-9ff1-2aa0e73e9d53)

### I.1. Fraud Transactions Dataset
The fraud transactions dataset contains information on a series of transactions, including the transaction date and time, credit card number, merchant, and transaction category. This report will provide an overview of the dataset and its columns, including the data types, number of unique values, and other statistical information.

This dataset is fictional and is trying to simulate real life details. Any similarity to real life cases is purely coincidental.
It has the following columns.

trans_date_trans_time: The date and time of the transaction.

- cc_num: credit card number.

- merchant: Merchant who was getting paid.

- category: In what area does that merchant deal.

- amt: Amount of money in American Dollars.

- first: first name of the card holder.

- last: last name of the card holder.

- gender: Gender of the cardholder.Just male and female!

- street:Street of card holder residence

- city:city of card holder residence

- state:state of card holder residence

- zip:ZIP code of card holder residence

- lat:latitude of card holder

- long:longitude of card holder

- city_pop:Population of the city

- job:trade of the card holder

- dob:Date of birth of the card holder

- trans_num: Transaction ID

- unix_time: Unix time which is the time calculated since 1970 to today.

- merch_lat: latitude of the merchant

- merch_long:longitude of the merchant

- is_fraud: Whether the transaction is fraud(1) or not(0)

However, due to the computer's limited capacity, I won't utilize all of these columns; instead, I'll focus on only the most influential ones. 


#### dataset info


``` 
fraud_train.info()
fraud_train.head()
fraud_train.describe()
```
![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/3508af43-e23a-4dc7-80bb-23cbedb58af8)
![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/5f15b516-f987-4ca0-b3fb-0a63799f76dc)
![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/0af8aaa7-39ed-476b-92a5-b59d2964a8fa)


```
fraud_test.info()
fraud_test.head()
fraud_test.describe()
```
![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/747f96d3-9dd9-40cc-82a1-30f8d7eba6af)
![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/1e79ee29-3758-4ab2-8f81-9db2409f36d1)
![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/04ba847c-de4c-4887-acc7-71eae4599e7d)


Correlations table: 

![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/df7da0f5-a4bc-4e68-8516-85626b4d9f07)

Count Missing value: 

![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/273d131b-e173-432a-9e5a-55faef55b3d8)

Count number of fraud transaction by category in train dataset: 

![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/7fa3bcf2-894c-4ab1-aaf8-c5240d145363)

Percentage of frad/non-frad transaction: 

![image](https://github.com/ThuHuong-Gina/Fraud-Detect-Transaction/assets/141025228/fbeb953c-06a2-4132-97c1-98b665a74171)







