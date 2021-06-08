# Analytics Vidhya Hackathon - Credit Card Lead Prediction

## Question
Happy Customer Bank is a mid-sized private bank that deals in all kinds of banking products, like Savings accounts, Current accounts, investment products, credit products, among other offerings. The bank also cross-sells products to its existing customers and to do so they use different kinds of communication like tele-calling, e-mails, recommendations on net banking, mobile banking, etc. In this case, the Happy Customer Bank wants to cross sell its credit cards to its existing customers. The bank has identified a set of customers that are eligible for taking these credit cards. 
Now, the bank is looking for your help in identifying customers that could show higher intent towards a recommended credit card, given: 
Customer details (gender, age, region etc.) Details of his/her relationship with the bank (Channel_Code, Vintage, Avg_Asset_Value etc.)

## Data dictionary
|   Variable    |  Description  |
| ------------- | ------------- |
|     ID        | Unique Identifier for a row  |
| Gender  | Gender of the Customer  |
|    Age    |   Age of the Customer (in Years)    |
| Region_Code | Code of the Region for the customers |
| Occupation | Occupation Type for the customer |
| Channel_Code | Acquisition Channel Code for the Customer (Encoded) |
| Vintage | Vintage for the Customer (In Months) |
| Credit_Product | If the Customer has any active credit product (Home loan,Personal loan, Credit Card etc.) |
| Avg_Account_Balance | Average Account Balance for the Customer in last 12 Months |
| Is_Active | If the Customer is Active in last 3 Months |
| Is_Lead(Target) | If the Customer is interested for the Credit Card , 0 : Customer is not interested , 1 : Customer is interested |

## Datasets: 
    1.	Train.csv
    2.	Test.csv

## Training Data Info:
 #   Column               Non-Null Count   Dtype 
---  ------               --------------   ----- 
 0   ID                   245725 non-null  object
 1   Gender               245725 non-null  object
 2   Age                  245725 non-null  int64 
 3   Region_Code          245725 non-null  object
 4   Occupation           245725 non-null  object
 5   Channel_Code         245725 non-null  object
 6   Vintage              245725 non-null  int64 
 7   Credit_Product       216400 non-null  object
 8   Avg_Account_Balance  245725 non-null  int64 
 9   Is_Active            245725 non-null  object
 10  Is_Lead              245725 non-null  int64 

## Testing Data Info
 #   Column               Non-Null Count   Dtype 
---  ------               --------------   ----- 
 0   ID                   105312 non-null  object
 1   Gender               105312 non-null  object
 2   Age                  105312 non-null  int64 
 3   Region_Code          105312 non-null  object
 4   Occupation           105312 non-null  object
 5   Channel_Code         105312 non-null  object
 6   Vintage              105312 non-null  int64 
 7   Credit_Product       92790 non-null   object
 8   Avg_Account_Balance  105312 non-null  int64 
 9   Is_Active            105312 non-null  object

# Step by step procedure

## Explore Data (Training and Test)
Exploratory data analysis is an approach of analysing data sets to summarize their main characteristics, often using statistical graphics and other data visualization methods. It is a critical process of performing initial investigations on data so as to discover patterns, to spot anomalies, to test hypothesis and to check assumptions with the help of summary statistics and graphical representations.
The major processes that we do in the EDA are:
    – Handling Missing values
    – Removing duplicates
    – Outlier Treatment
    – Normalizing and Scaling ( Numerical Variables)
    – Encoding Categorical variables ( Dummy Variables)
    – Bivariate Analysis
For the above process, some important libraries are imported,
    -	Numpy
    -	Pandas
    -	Seaborn and
    -	Matplotlip
    
    
  
