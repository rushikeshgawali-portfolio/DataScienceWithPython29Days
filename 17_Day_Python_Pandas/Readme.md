
## Introduction
In Data Science, data is often stored in:

Excel files
CSV files
Databases
Reports
Working with large amounts of data using Python lists can be difficult.

Pandas is a Python library used to load, clean, analyze, and manipulate data efficiently.

It is one of the most important tools for:

Data Analysis
Data Science
Machine Learning
Business Intelligence
Why Pandas is Important
Imagine you have a sales report with 10,000 rows.

You may want to:

Find total sales
Calculate average sales
Filter records
Remove missing values
Generate reports
Pandas helps perform these tasks quickly with just a few lines of code.

Real-Life Analogy
Think of Pandas as an Excel spreadsheet inside Python.

With Pandas, you can:

✅ Filter rows

✅ Sort data

✅ Calculate totals

✅ Find averages

✅ Clean messy data

Just like Excel, but much more powerful.

Installing Pandas
pip install pandas
Importing Pandas
import pandas as pd
pd is the standard alias used by Data Scientists.

What is a DataFrame?
A DataFrame is the main data structure in Pandas.

It looks like an Excel table.

import pandas as pd

data = {
    "Name": ["Rahul", "Priya", "Amit"],
    "Age": [21, 22, 20]
}

df = pd.DataFrame(data)

print(df)
Output:

    Name  Age
0  Rahul   21
1  Priya   22
2   Amit   20
Creating a DataFrame
import pandas as pd

students = {
    "Name": ["Rahul", "Priya"],
    "Marks": [85, 92]
}

df = pd.DataFrame(students)

print(df)
Reading a CSV File
Most Data Science datasets are stored as CSV files.

import pandas as pd

df = pd.read_csv("students.csv")

print(df.head())
Why?
You will use this daily as a Data Analyst or Data Scientist.

Viewing Data
First 5 Rows
print(df.head())
Last 5 Rows
print(df.tail())
Data Information
print(df.info())
Selecting Columns
print(df["Name"])
Output:

0 Rahul
1 Priya
2 Amit
Selecting Multiple Columns
print(df[["Name", "Marks"]])
Filtering Data
Students with Marks Greater Than 80
print(df[df["Marks"] > 80])
Output:

    Name  Marks
0  Rahul     85
1  Priya     92
Basic Data Analysis
Average Marks
print(df["Marks"].mean())
Maximum Marks
print(df["Marks"].max())
Minimum Marks
print(df["Marks"].min())
Total Marks
print(df["Marks"].sum())
Handling Missing Values
Check Missing Values
print(df.isnull().sum())
Fill Missing Values
df.fillna(0, inplace=True)
Missing values are very common in real-world datasets.

Sorting Data
Ascending Order
df.sort_values("Marks")
Descending Order
df.sort_values("Marks", ascending=False)
Pandas Indexing and Selection
Select First Row
print(df.iloc[0])
Select Multiple Rows
print(df.iloc[0:3])
Select Specific Rows and Columns
print(df.iloc[0:2, 0:2])
Real Data Science Example
import pandas as pd

sales = {
    "Month": ["Jan", "Feb", "Mar"],
    "Sales": [1200, 1500, 1800]
}

df = pd.DataFrame(sales)

print("Average Sales:", df["Sales"].mean())
print("Highest Sales:", df["Sales"].max())
print("Total Sales:", df["Sales"].sum())
Output:

Average Sales: 1500
Highest Sales: 1800
Total Sales: 4500
Pandas in a Data Science Workflow
Step 1: Load Data
df = pd.read_csv("sales.csv")
Step 2: Explore Data
df.head()
df.info()
Step 3: Clean Data
df.fillna(0)
Step 4: Analyze Data
df["Sales"].mean()
Step 5: Build Machine Learning Models
After cleaning and analysis, data is passed to machine learning libraries like Scikit-Learn.

How Pandas is Used in Data Science Jobs
Data Analyst
Create reports
Analyze sales data
Track KPIs
Clean business data
Data Scientist
Prepare datasets
Clean missing values
Analyze trends
Build machine learning models
Business Analyst
Study customer behavior
Generate dashboards
Analyze company performance
Machine Learning Engineer
Prepare and transform datasets
Feature engineering
Data preprocessing
Best Practices
✅ Import Pandas as pd
import pandas as pd
✅ Always Inspect Data First
df.head()
df.info()
✅ Handle Missing Values
df.fillna(0)
✅ Use Meaningful Column Names
Good:

Sales_Amount
Student_Marks
Avoid:

A
B
C
✅ Check Data Types
df.dtypes
✅ Save Cleaned Data
df.to_csv("clean_data.csv", index=False)
Beginner Practice Exercises
Exercise 1
Create a DataFrame containing:

Name
Age
City
Print the DataFrame.

Exercise 2
Create a student marks DataFrame and calculate:

Average marks
Highest marks
Lowest marks
Exercise 3
Read a CSV file using:

pd.read_csv()
Exercise 4
Filter students with marks greater than 80.

Exercise 5
Sort student marks from highest to lowest.

Mini Project: Employee Salary Analysis
import pandas as pd

data = {
    "Employee": ["Rahul", "Priya", "Amit"],
    "Salary": [25000, 30000, 28000]
}

df = pd.DataFrame(data)

print("Average Salary:", df["Salary"].mean())
print("Highest Salary:", df["Salary"].max())
print("Lowest Salary:", df["Salary"].min())
Summary
Pandas is the most popular library for data analysis in Python.
A DataFrame is like an Excel spreadsheet in Python.
Pandas helps load, clean, analyze, and transform data.
It is widely used by Data Analysts, Data Scientists, and Machine Learning Engineers.
Most real-world Data Science projects use Pandas.
