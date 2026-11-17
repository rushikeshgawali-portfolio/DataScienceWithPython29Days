## Data Cleaning Using Python
📖 Introduction
Data Cleaning is the process of preparing raw data by removing errors, handling missing values, correcting inconsistencies, and formatting data properly.

Clean data helps:

Improve data quality
Increase analysis accuracy
Build better machine learning models
Reduce errors in reporting
🎯 Why Data Cleaning is Important
Imagine a customer database:

Name	Age	City
John	25	New York
John	25	New York
Sarah	NaN	London
Mike	200	Toronto
Problems:

Duplicate records
Missing values
Invalid age values
Data cleaning helps fix these issues before analysis.

🛠 Common Data Cleaning Tasks
1. Handle Missing Values
Identify missing data:

import pandas as pd

df = pd.read_csv("data.csv")

print(df.isnull().sum())
Fill missing values:

df["Age"].fillna(df["Age"].mean(), inplace=True)
Remove rows with missing values:

df.dropna(inplace=True)
2. Remove Duplicate Records
Check duplicates:

print(df.duplicated().sum())
Remove duplicates:

df.drop_duplicates(inplace=True)
3. Rename Columns
Before:

print(df.columns)
Rename:

df.rename(columns={
    "Cust_Name": "Customer_Name",
    "Ph_No": "Phone_Number"
}, inplace=True)
4. Fix Data Types
Check data types:

print(df.dtypes)
Convert data type:

df["Age"] = df["Age"].astype(int)
Convert date column:

df["Date"] = pd.to_datetime(df["Date"])
5. Handle Outliers
Example:

import numpy as np

Q1 = df["Salary"].quantile(0.25)
Q3 = df["Salary"].quantile(0.75)

IQR = Q3 - Q1

lower = Q1 - 1.5 * IQR
upper = Q3 + 1.5 * IQR

df = df[(df["Salary"] >= lower) &
        (df["Salary"] <= upper)]
6. Remove Extra Spaces
Before cleaning:

df["Name"]
Output:

" John "
Clean spaces:

df["Name"] = df["Name"].str.strip()
7. Standardize Text Values
Before:

Male
male
MALE
After:

df["Gender"] = df["Gender"].str.lower()
Output:

male
male
male
8. Handle Incorrect Values
Find invalid ages:

df[df["Age"] > 100]
Replace values:

df.loc[df["Age"] > 100, "Age"] = 100
📊 Useful Pandas Functions
Function	Purpose
isnull()	Check missing values
fillna()	Fill missing values
dropna()	Remove missing values
duplicated()	Find duplicates
drop_duplicates()	Remove duplicates
astype()	Change data type
rename()	Rename columns
replace()	Replace values
strip()	Remove spaces
to_datetime()	Convert dates
✅ Complete Example
import pandas as pd

# Load dataset
df = pd.read_csv("employees.csv")

# Remove duplicates
df.drop_duplicates(inplace=True)

# Fill missing age values
df["Age"].fillna(df["Age"].mean(), inplace=True)

# Remove extra spaces
df["Name"] = df["Name"].str.strip()

# Convert gender to lowercase
df["Gender"] = df["Gender"].str.lower()

# Convert joining date
df["Joining_Date"] = pd.to_datetime(df["Joining_Date"])

print(df.head())
💡 Best Practices
Always inspect data before cleaning.
Keep a backup of raw data.
Document every cleaning step.
Verify data types after conversion.
Handle missing values carefully.
Validate results after cleaning.
📝 Summary
Data Cleaning is a critical step in the data analysis workflow. It ensures that datasets are accurate, consistent, and ready for analysis. Using Python and Pandas, we can efficiently handle missing values, duplicates, incorrect formats, outliers, and inconsistent data.

Key Takeaways
Clean data produces reliable results.
Pandas provides powerful data-cleaning tools.
Always validate your cleaned dataset.
Data cleaning often takes 60-80% of a data analyst's time.
Happy Learning! 🚀
