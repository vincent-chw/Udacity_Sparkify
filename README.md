# Udacity_Sparkify
Udacity Capstone

Project Motivation
Churn prediction is a crucial task in data science, as it helps businesses identify customers who are likely to leave and take actions to retain them. By analyzing historical data on customer behaviour, a churn prediction model can identify patterns and trends that indicate a high risk of churn. This allows a company to take proactive measures to retain at-risk customers, such as offering promotions or providing personalized customer service. Overall, churn prediction can help companies increase revenue and customer loyalty by reducing customer turnover.

File Descriptions
Udacity_Sparkify.ipynb contains the codes from start to finish. 

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

Modeling
Three different models which are suitable for classification problems shall be trained on the dataset and the performance shall be compared to determine the best performing model. 

Conclusion
Due to the imbalanced nature of the dataset (User who churned << User who did not churn), the F1 score is used as the performance criteria. The results show that the Random Forest model obtained the highest F1 score. 

My Medium blog post can be found in the link below:
https://vincent-chw.medium.com/predicting-customer-churn-using-pyspark-on-amazon-emr-dd0e9fbe8abd

Libraries used:
aws-cfn-bootstrap          2.0

beautifulsoup4             4.9.3

joblib                     1.2.0

matplotlib                 3.5.3

numpy                      1.20.0

packaging                  23.0

pandas                     1.0.5

pip                        20.2.2

