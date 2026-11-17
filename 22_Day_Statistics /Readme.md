## Statistics for Data Science
## 📖 Introduction
Statistics is the science of collecting, organizing, analyzing, interpreting, and presenting data.

In Data Science, statistics helps us:

Understand data
Discover patterns and trends
Make predictions
Test hypotheses
Support decision-making
Without statistics, data is just a collection of numbers with little meaning.

🎯 Why Statistics is Important in Data Science
Data Scientists use statistics to:

✅ Summarize data

✅ Identify patterns

✅ Understand relationships

✅ Build machine learning models

✅ Make data-driven decisions

✅ Measure uncertainty

Real-World Example
An e-commerce company wants to know:

Which product sells the most?
What is the average order value?
Which customers are likely to buy again?
Statistics provides tools to answer these questions.

Types of Statistics
Statistics is divided into two major categories:

1. Descriptive Statistics
Descriptive Statistics summarizes and describes data.

Example
Student Marks:

70, 75, 80, 85, 90
We can calculate:

Mean
Median
Mode
Range
Standard Deviation
These values help understand the dataset quickly.

2. Inferential Statistics
Inferential Statistics uses sample data to make predictions about a larger population.

Example
Survey:

100 people surveyed
Using survey results, we estimate the opinions of:

10,000 customers
Inferential statistics helps make predictions and decisions.

Key Statistical Terms
Population
The entire group being studied.

Example
All customers of Amazon.

Sample
A smaller group selected from the population.

Example
1,000 customers chosen from all Amazon customers.

Variable
A characteristic being measured.

Examples:

Age
Salary
Height
Weight
Observation
A single data record.

Example:

Name	Age
John	25
This row is one observation.

Measures of Central Tendency
These measures identify the center of a dataset.

1. Mean (Average)
Formula:

Mean = Sum of Values / Number of Values
Example:

10, 20, 30, 40, 50
Calculation:

Mean = (10+20+30+40+50)/5

Mean = 30
Python Example:

import numpy as np

data = [10,20,30,40,50]

print(np.mean(data))
Output:

30
2. Median
Middle value of sorted data.

Example:

10,20,30,40,50
Median:

30
Python Example:

import numpy as np

print(np.median(data))
3. Mode
Most frequently occurring value.

Example:

10,20,20,30,40
Mode:

20
Python Example:

from scipy import stats

data = [10,20,20,30,40]

print(stats.mode(data))
Measures of Dispersion
These measure how spread out data is.

1. Range
Formula:

Range = Maximum - Minimum
Example:

10,20,30,40,50
Range:

50 - 10 = 40
2. Variance
Measures data variability around the mean.

Python Example:

import numpy as np

data = [10,20,30,40,50]

print(np.var(data))
3. Standard Deviation
Measures how far values are from the mean.

Python Example:

import numpy as np

data = [10,20,30,40,50]

print(np.std(data))
Probability Basics
Probability measures the likelihood of an event occurring.

Formula:

Probability = Favorable Outcomes / Total Outcomes
Example:

Rolling a dice.

Probability of getting 3

= 1/6
Data Distribution
A distribution shows how data values are spread.

Normal Distribution
A bell-shaped distribution where:

Most values are near the mean
Fewer values exist at extremes
Examples:

Heights
Exam scores
IQ scores
Skewed Distribution
Right Skewed
Mean > Median
Examples:

Income
House prices
Left Skewed
Mean < Median
Examples:

Easy exam scores
Percentiles
Percentiles indicate relative standing in data.

Example:

90th Percentile
Means:

90% of values are below that score.
Example Applications:

Competitive exams
Employee performance
Customer segmentation
Correlation
Correlation measures the relationship between variables.

Positive Correlation
When one variable increases, the other increases.

Example:

Study Hours ↑
Marks ↑
Negative Correlation
When one variable increases, the other decreases.

Example:

Exercise ↑
Body Fat ↓
No Correlation
No relationship exists.

Example:

Shoe Size and Salary
Python Example:

import pandas as pd

df.corr(numeric_only=True)
Hypothesis Testing
Hypothesis testing helps determine whether a claim is statistically significant.

Null Hypothesis (H0)
Assumes no effect or no difference.

Example:

New medicine has no effect.
Alternative Hypothesis (H1)
Assumes a significant effect exists.

Example:

New medicine improves patient health.
Statistical Tests
T-Test
Used to compare means of two groups.

Examples:

Male vs Female salary
Two marketing campaigns
Chi-Square Test
Used for categorical data.

Examples:

Product preference
Survey responses
ANOVA
Used to compare multiple groups.

Example:

Compare sales of 3 stores.
Statistics in Machine Learning
Statistics is used in:

Data Cleaning
Feature Engineering
Data Visualization
Model Evaluation
Probability Models
Predictive Analytics
A/B Testing
Examples:

Linear Regression
Logistic Regression
Naive Bayes
Decision Trees
Useful Python Libraries
NumPy
import numpy as np

np.mean(data)
np.median(data)
np.std(data)
Pandas
import pandas as pd

df.describe()
SciPy
from scipy import stats
Used for:

Hypothesis Testing
Statistical Analysis
Probability Functions
✅ Complete Example
import pandas as pd
import numpy as np

scores = [70, 75, 80, 85, 90]

print("Mean:", np.mean(scores))
print("Median:", np.median(scores))
print("Standard Deviation:", np.std(scores))
print("Maximum:", np.max(scores))
print("Minimum:", np.min(scores))
Output:

Mean: 80.0
Median: 80.0
Standard Deviation: 7.07
Maximum: 90
Minimum: 70
💡 Best Practices
Understand data before analysis.
Always visualize data.
Check for outliers.
Use appropriate statistical tests.
Validate assumptions before modeling.
Interpret results carefully.
Combine statistics with domain knowledge.
🌍 Real-World Applications
Healthcare Analytics
Business Intelligence
Finance and Banking
Marketing Analytics
Sports Analytics
Manufacturing
Machine Learning
Artificial Intelligence
📝 Summary
Statistics is the foundation of Data Science. It helps us understand data, identify patterns, make predictions, and support decision-making. Every Data Scientist relies on statistical concepts such as mean, median, variance, probability, correlation, and hypothesis testing to analyze data effectively.

Key Takeaways
Statistics turns raw data into useful insights.
Descriptive statistics summarizes data.
Inferential statistics makes predictions.
Probability helps measure uncertainty.
Correlation identifies relationships.
Hypothesis testing validates assumptions.
Statistics is essential for Machine Learning and Data Science.
Happy Learning! 📊🚀
