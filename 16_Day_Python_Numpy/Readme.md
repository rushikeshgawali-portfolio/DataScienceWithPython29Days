
## Introduction
As a Data Scientist, you will often work with:

Thousands of rows of data
Numerical calculations
Statistics
Machine Learning datasets
Data cleaning and transformation
Performing these tasks with normal Python lists can be slow and inconvenient.

NumPy (Numerical Python) is a powerful Python library used for fast numerical computing and data analysis.

It is one of the most important libraries in the Data Science ecosystem and is commonly used with:

Pandas
Matplotlib
Scikit-Learn
TensorFlow
PyTorch
Why NumPy is Important in Data Science
Imagine you work as a Data Analyst in a company.

You have sales data like:

100
200
150
300
250
You may want to:

Calculate the average sales
Find the highest and lowest sales
Perform mathematical calculations
Analyze thousands of records quickly
NumPy makes these tasks much easier and faster.

Real-Life Analogy
Think of NumPy as a calculator designed for handling huge amounts of data.

Normal Calculator
Can calculate:

10 + 20
NumPy Calculator
Can calculate:

1000 values at once
That's why Data Scientists use NumPy.

Installing NumPy
pip install numpy
Verify installation:

import numpy as np

print(np.__version__)
Importing NumPy
By convention:

import numpy as np
Why use np?

Because:

np.array()
np.mean()
np.sum()
is shorter than:

numpy.array()
numpy.mean()
numpy.sum()
What is a NumPy Array?
A NumPy array is similar to a Python list but:

✅ Faster

✅ Uses less memory

✅ Supports advanced mathematical operations

Python List Example
numbers = [10, 20, 30, 40]

print(numbers)
Output:

[10, 20, 30, 40]
NumPy Array Example
import numpy as np

numbers = np.array([10, 20, 30, 40])

print(numbers)
Output:

[10 20 30 40]
Creating NumPy Arrays
1. One-Dimensional Array
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)
Output:

[1 2 3 4 5]
2. Two-Dimensional Array
Think of it like an Excel table.

import numpy as np

arr = np.array([
    [1, 2, 3],
    [4, 5, 6]
])

print(arr)
Output:

[[1 2 3]
 [4 5 6]]
Array Properties
import numpy as np

arr = np.array([
    [1, 2, 3],
    [4, 5, 6]
])

print(arr.shape)
Output:

(2, 3)
Meaning:

2 rows
3 columns
Common Data Science Operations
Sum
Calculate total sales.

import numpy as np

sales = np.array([100, 200, 150, 300])

print(np.sum(sales))
Output:

750
Average
Find average sales.

print(np.mean(sales))
Output:

187.5
Maximum Value
print(np.max(sales))
Output:

300
Minimum Value
print(np.min(sales))
Output:

100
Performing Calculations
Add 10 to Every Value
import numpy as np

prices = np.array([100, 200, 300])

new_prices = prices + 10

print(new_prices)
Output:

[110 210 310]
This is called Vectorized Operations.

A Data Scientist uses this all the time.

Why NumPy is Faster Than Python Lists
Python List:

prices = [100, 200, 300]

new_prices = []

for price in prices:
    new_prices.append(price + 10)
NumPy:

prices = np.array([100, 200, 300])

new_prices = prices + 10
Fewer lines of code and much faster.

Generating Arrays Automatically
Create Numbers from 1 to 10
import numpy as np

arr = np.arange(1, 11)

print(arr)
Output:

[1 2 3 4 5 6 7 8 9 10]
Create Zeros
import numpy as np

arr = np.zeros(5)

print(arr)
Output:

[0. 0. 0. 0. 0.]
Create Ones
import numpy as np

arr = np.ones(5)

print(arr)
Output:

[1. 1. 1. 1. 1.]
Data Science Example: Student Marks Analysis
import numpy as np

marks = np.array([75, 80, 90, 65, 85])

print("Average:", np.mean(marks))
print("Highest:", np.max(marks))
print("Lowest:", np.min(marks))
Output:

Average: 79.0
Highest: 90
Lowest: 65
Real-World Use
As a Data Analyst, you might:

Analyze student performance
Measure employee productivity
Evaluate sales trends
Create business reports
Working with Multi-Dimensional Data
Employee salary data:

import numpy as np

salary = np.array([
    [25000, 27000, 30000],
    [35000, 38000, 40000]
])

print(salary)
Output:

[[25000 27000 30000]
 [35000 38000 40000]]
Think of this as an Excel spreadsheet stored in Python.

NumPy and Data Science Workflow
A typical Data Scientist uses NumPy for:

Step 1: Load Data
import numpy as np
Step 2: Store Data
sales = np.array([100, 200, 300])
Step 3: Analyze Data
np.mean(sales)
np.max(sales)
np.min(sales)
Step 4: Prepare Data for Machine Learning
sales * 1.10
This can increase all values by 10%.

Best Practices
✅ Use NumPy for Numerical Data
Good:

sales = np.array([100, 200, 300])
Avoid large calculations using regular lists.

✅ Import Using Alias
import numpy as np
Industry standard practice.

✅ Use Vectorized Operations
Good:

sales = sales + 10
Avoid:

for sale in sales:
    print(sale + 10)
for large datasets.

✅ Use Built-In Functions
np.mean()
np.sum()
np.max()
np.min()
Cleaner and faster.

✅ Keep Arrays Consistent
Try to store similar types of values together.

Good:

np.array([10, 20, 30])
Less ideal:

np.array([10, "Hello", 30])
Beginner Practice Exercises
Exercise 1
Create a NumPy array containing:

10, 20, 30, 40, 50
Print the array.

Exercise 2
Find:

Sum
Average
Maximum
Minimum
of the array.

Exercise 3
Create a NumPy array of student marks and calculate the average score.

Exercise 4
Create an array using:

np.arange(1, 21)
Print the result.

Exercise 5
Increase every value in this array by 5.

[10, 20, 30, 40]
Mini Project: Monthly Sales Analysis
import numpy as np

sales = np.array([
    1200,
    1500,
    1800,
    1700,
    2100,
    2500
])

print("Total Sales:", np.sum(sales))
print("Average Sales:", np.mean(sales))
print("Highest Sales:", np.max(sales))
print("Lowest Sales:", np.min(sales))
Sample Output
Total Sales: 10800
Average Sales: 1800
Highest Sales: 2500
Lowest Sales: 1200
How NumPy Helps in a Data Science Career
Data Analyst
Analyze business data
Create reports
Calculate KPIs
Data Scientist
Prepare datasets
Perform statistical calculations
Build machine learning models
Machine Learning Engineer
Process large numerical datasets
Feed data into AI models
Business Analyst
Analyze trends and patterns
Support decision-making
Summary
NumPy stands for Numerical Python.
It is the foundation of Data Science in Python.
NumPy arrays are faster and more efficient than Python lists.
NumPy provides built-in functions for calculations and data analysis.
Data Scientists use NumPy to clean, process, and analyze data.
NumPy works seamlessly with Pandas, Matplotlib, and Machine Learning libraries.
