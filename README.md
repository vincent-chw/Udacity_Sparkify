# Udacity_Sparkify
Udacity Capstone

Installations


Project Motivation


File Descriptions


How to Interact with your project


Licensing, Authors, Acknowledgements

Predicting Customer Churn Using Pyspark

This project aims to predict which customer will churn based on the dataset of the customers. Being able to predict customer churn is very important in a business sense because it is much cheaper to retain an existing customer than acquiring a new customer. Therefore, if we are able to predict a customer having a high chance of churning, steps can be taken to try to prevent the customer from churning. 

The dataset is provided by Udacity for the Data Scienctist Capstone Project. 

For large dataset, PySpark is used for the entire process: 
1. Exploratory data analysis
2. Data cleaning
3. Feature engineering
4. Modeling

Exploratory Data Analysis
The project starts with some exploratory data analysis of the dataset. It can be seen that the data is imbalanced in terms of customers who churned vs customers who did not churn. Care will need to be taken when dealing with imbalanced data. 

Data Cleaning
The data cleaning process involves removing columns that does not contribute to the prediction of customer churn, dealing with missing values, and converting the timestamp to a proper datetime that makes sense. 

Feature Engineering
The features that holds the most promise in being able to predict churn would be related to customer's behaviour. Hence, for each customer, the average page visits based on the total number of days shall be calculated and recorded. 
