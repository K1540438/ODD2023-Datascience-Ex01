# Ex-01_DS_Data_Cleansing


## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file

# CODE and OUTPUT
```
import pandas as pj
df1=pj.read_csv("Loan_data.csv")
print(df1)
df1.isnull().sum()
df1['Gender']=df1['Gender'].fillna(df1['Gender'].mode()[0])
df1['Married']=df1['Married'].fillna(df1['Married'].mode()[0])
df1['Dependents']=df1['Dependents'].fillna(df1['Dependents'].mode()[0])
df1['Education']=df1['Education'].fillna(df1['Education'].mode()[0])
df1['Self_Employed']=df1['Self_Employed'].fillna(df1['Self_Employed'].mode()[0])
df1['LoanAmount']=df1['LoanAmount'].fillna(df1['LoanAmount'].mode()[0])
df1['Loan_Amount_Term']=df1['Loan_Amount_Term'].fillna(df1['Loan_Amount_Term'].mode()[0])
df1['Credit_History']=df1['Credit_History'].fillna(df1['Credit_History'].mode()[0])
df1.isnull().sum()

import pandas as pj
df1=pj.read_csv("Data_set.csv")
print(df1)
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
print(df['show_name'])
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
print(df['aired_on'])
df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0])
print(df['original_network'])
df['rating']=df['rating'].fillna(df['rating'].mean())
print(df['rating'])
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
print(df['current_overall_rank'])
df['watchers']=df['watchers'].fillna(df['watchers'].median())
print(df['watchers'])
df.isnull().sum()
df.info()
```
##output

<img width="364" alt="Screenshot 2023-08-23 160056" src="https://github.com/K1540438/ODD2023-Datascience-Ex01/assets/84171243/d4ce6aaa-34e9-4944-b900-8589adb8b0d2">

<img width="227" alt="Screenshot 2023-08-23 160116" src="https://github.com/K1540438/ODD2023-Datascience-Ex01/assets/84171243/9b84eb47-d353-4b5f-9a99-aad85543285e">


<img width="236" alt="Screenshot 2023-08-23 160126" src="https://github.com/K1540438/ODD2023-Datascience-Ex01/assets/84171243/7eb04c32-6829-4967-9f61-efe41b40fc10">
