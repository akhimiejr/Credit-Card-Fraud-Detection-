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
## 3.1.1 Data Cleaning 
The dataset was thoroughly examined for missing values, duplicates, and outliers. Missing 
values were imputed using appropriate techniques and removed when they constituted a 
significant portion of the data. Duplicate transactions were identified and removed to avoid 
redundancy and skewed results. 
## 3.1.2 Data Transformation 
Categorical variables were encoded using techniques such as one-hot encoding or label 
encoding to make them suitable for analysis. The encoded numerical variable is_fraud was 
replaced by a new binary variable that is for the unique integer value. 
## 3.1.3 Data Subsetting 
The data set is about 1.8 million observations and this quite large and will cause performance 
issues when running the analysis. To resolve this issue, a subset of the data was taken. This was 
done by looking at the top ten highest transaction by state and the top ten highest fraudulent 
transaction. New York was the state with the highest fraudulent transaction and had the second 
highest transaction. Our focus moving forward will be focused on the state of New York.

![image](https://github.com/user-attachments/assets/ce4ea6c1-9b39-4665-9b07-29f1d3213e21)

![image](https://github.com/user-attachments/assets/1350a85f-f675-4fc2-aca7-21f989049678)

# 3.2 Exploratory Data Analysis 
To gain insights into the characteristics of the credit card fraud dataset and identify potential 
patterns and relationships an exploratory data analysis (EDA) techniques were employed.  
As shown in the previous fig  
• Non-Fraudulent Transactions: Texas (TX) has the highest number of non-fraudulent 
transactions (134,677) and total transaction amount ($9,239,298), followed by New York 
(NY) and California (CA). 
• Fraudulent Transactions: New York (NY) leads in fraudulent transactions both in count 
(730) and total amount ($395,295), followed by Texas (TX) and Pennsylvania (PA). 
## 3.2.1 Distribution Analysis 
EDA was carried out to gain a broad understanding of the dataset's features and attributes and 
uncover potential relationships between variables. Summary statistics, such as mean, median, 
and standard deviation, were calculated for numerical variables, while frequency distributions 
were examined for categorical variables. 

![image](https://github.com/user-attachments/assets/e3d05276-8fd4-4336-ad54-f196aa539ffc)

Fig 3.3 Summary Statistics of Gender with regards to transaction population and age. 

![image](https://github.com/user-attachments/assets/3a51f3bd-5d2a-4211-bee5-b6c2483c72ab)

Fig 3.4 Average spend and number of transactions by gender. 

The above table shows the average amount spent by customer gender. On average Male 
customer spend more money per transaction when compared to female customer and the 
overall average. However, female customers carry out more transactions and in essence spend 
more money overall.  
To understand the age distribution of the customers using credit card a box plot is shown in the 
below figure. 

![image](https://github.com/user-attachments/assets/5d5ec8d8-6a2a-4041-bcfa-5eb24b6634d1)

In the above figure, it can be observed that on average the male customers are older than the 
female customer. With the female customer on average being in their forties and the male 
customers are in their fifties. Another trend that can be observed from the figure is that 
fraudulent transactions tend to happen in both genders. This can be alluded to the fact that 
older individuals are more susceptible to falling for scam as they are not technologically as 
savvy as their younger counterparts. This insight os quite significant as stakeholders in the 
customer experience team can use this detial and reach out to older customers especially, 
giving them training on how to spot fraudulent transactions there by curbing the risk of them 
falling victim to scam. 

![image](https://github.com/user-attachments/assets/3909539a-76f2-4338-81c1-edaa6bebd20f)

The above figure shows the frequency of legtimate transaction and the week day in which they 
occur the most. Monday and Sunday are the days where most transaction takes place and this 
is regardless of the gender making the transaction. This insight will enable stakeholders allocate 
resources to begining of the week and ensure there are no failures.

![image](https://github.com/user-attachments/assets/28a511f4-317b-4ba7-b290-b440e0a5a583)

In contrast to fig 3.6 the above figure shows that fraudulent transactions for male customers 
exceeds that of female customers from Wednesday to Saturday. However, fraudulent 
transaction mostly take place from Sunday to Tuesday for female customer. The spike days for 
fraudulent transactions are mostly Sundays and affect female customers the most. This insight 
can be utilized to educate customers with what to look out for with regards to fraudulent 
activities on their credit card. 

![image](https://github.com/user-attachments/assets/02e4adfe-17a7-4263-8b33-df3e1c3afdc1)

Fig 3.8 gives us insights into customer spending habits. We can see from the table that female 
customer out spends the male customers in every category except Travel. The highest category 
where customers spend their money is in Grocery point of sale i.e. where they physically swipe 
their card at the counter. The least amount spent in a category was also in grocery, but the 
payment method is online. It will make sense to market travel insurance to male customer and 
market coupons to female customers who physically shop for Grocery items

![image](https://github.com/user-attachments/assets/f25ce19b-75d4-49e5-bdcc-6dd55a64c949)

Fig 3.9 is a bar graph that splits the total transaction amount into the different category which 
customers carried out transaction. It can be seen that the bulk of the transaction was done in 
the grocery category. While shopping online had the most fraudulent transactions followed by 
miscellaneous shopping online. This is a good insight as stake holders can flag easily a 
transaction to be fraudulent when it falls into these categories and a warning message alerting 
the customer can be sent. 

![image](https://github.com/user-attachments/assets/e384f337-dfc4-4d78-90aa-b2d4969bb91f)

To understand the spending habit of customers the table in fig 3.10 was created, it shows that 
personal care and online grocery shopping are the two least categories where customers spend 
their money. On average, the least amount spend by a customer is on personal care but the 
most amount spent on average falls within the travel and physical grocery category. When 
compared to the median spent by customers the story slightly changes, miscellaneous and 
shopping but in physical stores and online shopping categories were the least amount were 
customers spend their money.

## 3.2.2 Time Series Analysis 
To understand the difference in characteristics of fraudulent transactions and non-fraudulent 
transactions, a time series analysis of both kinds of transactions was carried out. This will 
create a clear differentiation between what is considered to be fraudulent transactions and 
what is not. 

![image](https://github.com/user-attachments/assets/bdbc6890-d380-451f-a9c5-671e777c652d)

The figure above shows fraudulent transactions plotted by the hour of the day in which the 
transaction occurred. Instantly a theme can be seen, the scammers that carry out fraudulent 
transactions do so in the late hours of the day into the early hours of the day. This kind of 
information already gives a good red flag of when transactions can be halted if suspected of 
fraudulent activities. 

![image](https://github.com/user-attachments/assets/fdb17660-3db8-4515-a15c-182f537883af)

Fig 3.12 shows the hours in which customers carried out transactions by both male and female. 
There is an even spread of the data, with peak periods starting at mid-day and least transactions 
happening at midnight. When fig 3.12 is compared to fig 3.11, it is clear how fraudulent 
transactions can be profiled and as such detected using the hour of the day as a feature in a 
model that will predict fraudulent transactions. 
## 3.2.3 Correlation Analysis 
To effectively predict fraud, a correlation analysis was carried out using the amount spent by a 
customer and the likelihood of fraud to be committed. To achieve this, the amount being spent 
by customers were broken down into bins of eight. Each been representing a fraction of the total 
amount spent. The range of the bins are $20, $40, $100, $200, $500, $1,000, and above $1,000. 
The table shows that as the amount of money spent increases so does the likelihood of the 
transaction to be fraudulent. 
Fig 3.13 Table showing increase in amount spent and the likelihood

![image](https://github.com/user-attachments/assets/ca3cb97d-013c-435a-8b78-b8cfc97e0ab8)

![image](https://github.com/user-attachments/assets/6e381b9f-e94a-4dc7-9e1f-e73660fabe38)

Our earlier analysis showed that the average amount spent on any transaction by a customer, 
either female or male was $71, however when you look at fig 3.14, which is a characteristic of 
fraudulent transactions, the observation is that fraudulent transactions tend to be three times 
or higher the average spend of a customer. This makes sense as scammers would want to cash 
in big in order to get away with as much more as they can.  
## 3.2.3 Customer Age Analysis 
At the beginning of our analysis, we did a distribution of age within the customer base using the 
credit card. This showed that older customers tend to get defrauded. The below table is a 
comprehensive analysis of age of customers and the likelihood of getting defrauded. Just like 
we did with the correlation analysis, we will group the customer base into age range. Teenagers, 
customers below the age of 20 years old, Young Adults, customers between the age of 20 – 35 
years old, middle age between 35 and 60 years old, and then lastly Elderly, customers older 
than 60 years. This grouping will also be further grouped into gender, so we can have a clear 
view of how the age structure is between genders as well. The below figure shows in clear 
details this analysis.

![image](https://github.com/user-attachments/assets/e30d4ad9-15a5-4344-85aa-b85f5c7ef0f1)

![image](https://github.com/user-attachments/assets/9cc231be-9766-4d44-b350-a05b4261621a)

Imploring a bar graph to assist in buttressing the insight of our analysis, we can see that middled 
aged male customer are the most defrauded within our customer base followed by elderly 
women and young women. Teenage male customers also tend to fall victim as well.

# Conclusion 
This study aimed to analyse a credit card fraud dataset to gain insights into patterns and 
characteristics that can aid in the detection and prevention of fraudulent activities. Through 
exploratory data analysis using SAS and Tableau, several key findings were uncovered. 
The analysis revealed that certain factors, such as transaction amount, customer age, gender, 
and time of day, can be indicators of potential fraud. Fraudulent transactions were found to be 
more prevalent among older customers, suggesting a need for targeted education and 
awareness campaigns. Additionally, fraudulent activities were more likely to occur during late
night and early-morning hours, providing a temporal pattern that can be leveraged for fraud 
detection models. 
The critical comparison between SAS and Tableau highlighted the strengths and weaknesses of 
each tool concerning different aspects of fraud analytics. While SAS excelled in data 
manipulation, statistical analysis, and model building, Tableau demonstrated its prowess in 
interactive data visualization and user-friendly exploration. 
The insights gained from this study can be valuable for financial institutions and other 
organizations in developing robust fraud prevention strategies, optimizing resource allocation, 
and enhancing customer education and support.








