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

Modeling
Three different models which are suitable for classification problems shall be trained on the dataset and the performance shall be compared to determine the best performing model. 

Conclusion
Due to the imbalanced nature of the dataset (User who churned << User who did not churn), the F1 score is used as the performance criteria. The results show that the Random Forest model obtained the highest F1 score. 


Libraries used:
aws-cfn-bootstrap          2.0
beautifulsoup4             4.9.3
boto                       2.49.0
click                      8.1.3
cycler                     0.11.0
docutils                   0.14
fonttools                  4.38.0
jmespath                   1.0.1
joblib                     1.2.0
kiwisolver                 1.4.4
lockfile                   0.11.0
lxml                       4.9.1
matplotlib                 3.5.3
mysqlclient                1.4.2
nltk                       3.7
nose                       1.3.4
numpy                      1.20.0
packaging                  23.0
pandas                     1.0.5
Pillow                     9.4.0
pip                        20.2.2
py-dateutil                2.2
pyparsing                  3.0.9
pystache                   0.5.4
python-daemon              2.2.3
python-dateutil            2.8.2
python37-sagemaker-pyspark 1.4.2
pytz                       2022.6
PyYAML                     5.4.1
regex                      2021.11.10
setuptools                 28.8.0
simplejson                 3.2.0
six                        1.13.0
tqdm                       4.64.1
typing-extensions          4.4.0
wheel                      0.29.0
windmill                   1.6
