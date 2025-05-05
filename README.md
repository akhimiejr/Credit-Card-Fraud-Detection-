# Credit-Card-Fraud-Detection-
## 1 Introduction 
# 1.1 Aim and Objectives 
The primary aim of this study is to analyse a credit card fraud dataset to the identify patterns 
and gain a comprehensive insight that can aid in the detection and prevention of fraudulent 
activities. This will assist the banking industry in making critical step by which their 
customers use their credit card for transactions.  
The transaction data set that is being explored will also assist the company in exploring their 
customer spending habits, age groups that transact the most, time period where transactions 
occur, helping the company plan resource allocation there by optimising response time from 
their customer care departments (Author, 2024). 
The objectives that will be carried out in this study are as follows: 
1. Perform exploratory data analysis on the fraud dataset to understand the nature and 
characteristics of the data. 
2. Identify key factors and variables that contribute to the likelihood of fraudulent 
transactions. 
3. Develop strategies and techniques for detecting and preventing fraud based on the insights 
gained from the analysis. 
4. Compare the effectiveness and efficiency of SAS and Tableau in performing fraud 
analytics and data visualization. 
# 1.2 Background Information 
Fraud is a pervasive issue that affects businesses across various industries, leading to 
significant financial losses and reputational damage. With the advent of digital transactions 
and e-commerce, the risk of fraud has escalated, necessitating robust fraud detection and 
prevention mechanisms. This study aims to leverage data analytics and historical transaction 
data to uncover insights and develop robust fraud prevention strategies and anomalies that 
can indicate fraudulent activities, thereby enabling organizations to take proactive measures 
to mitigate fraud risks (Author, 2024).. 
# 1.3 Description of the Fraud Dataset 
The fraud dataset used in this study is a comprehensive collection of 1,852,394 transactions, 
which was obtained from the Kaggle website. The data set comprises of 23 variables 
representing various attributes of financial transactions including both legitimate and 
fraudulent transactions. The data set also captures transaction amount, customer 
demographics, geographic location, transaction time, and customer details like, date of birth, 
occupation, and gender. Table 1 below highlights the important variable that will aid the 
analysis and detection of fraud.

![image](https://github.com/user-attachments/assets/3b4a3f92-f719-4d29-9b97-691962702e01)

# 2. Analytics Design 
The analytics design employed in this study follows a structured approach, incorporating 
various data mining techniques and statistical methodologies. The process begins with data 
preprocessing, which involves cleaning and transforming the raw data to ensure its quality and 
suitability for analysis. Subsequently, exploratory data analysis (EDA) is conducted to gain a 
deeper understanding of the dataset's characteristics and identify potential relationships 
between variables. 
To illustrate the analytics design process, a Unified Modelling Language (UML) activity diagram 
is presented below:

![image](https://github.com/user-attachments/assets/53135cf9-9f56-46f7-8b61-48ae301a4792)

# 3. Data Analytics 
Tableau Desktop and SAS academy were the analytic used to analyse and carry out the 
prediction of fraud in this section.  
# 3.1 Data Pre-Processing 
Before proceeding with the analysis, several data pre-processing steps were performed to 
ensure the quality and consistency of the data. 
# 3.1.1 Data Cleaning 
The dataset was thoroughly examined for missing values, duplicates, and outliers. Missing 
values were imputed using appropriate techniques and removed when they constituted a 
significant portion of the data. Duplicate transactions were identified and removed to avoid 
redundancy and skewed results. 
# 3.1.2 Data Transformation 
Categorical variables were encoded using techniques such as one-hot encoding or label 
encoding to make them suitable for analysis. The encoded numerical variable is_fraud was 
replaced by a new binary variable that is for the unique integer value. 
# 3.1.3 Data Subsetting 
The data set is about 1.8 million observations and this quite large and will cause performance 
issues when running the analysis. To resolve this issue, a subset of the data was taken. This was 
done by looking at the top ten highest transaction by state and the top ten highest fraudulent 
transaction. New York was the state with the highest fraudulent transaction and had the second 
highest transaction. Our focus moving forward will be focused on the state of New York.
