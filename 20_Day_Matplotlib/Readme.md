Matplotlib
📖 Introduction
Matplotlib is one of the most popular Python libraries used for data visualization. It helps transform raw data into charts, graphs, and plots that are easier to understand and analyze.

Matplotlib is widely used by:

Data Analysts
Data Scientists
Machine Learning Engineers
Researchers
Students
It serves as the foundation for many other visualization libraries such as Seaborn.

🎯 Why Use Matplotlib?
Without visualization, data appears as numbers and tables.

Example:

Month	Sales
Jan	1000
Feb	1200
Mar	1500
Apr	1800
A graph instantly shows:

Growth trends
Patterns
Comparisons
Insights
Matplotlib makes this visualization possible.

🚀 Installation
Install Matplotlib using pip:

pip install matplotlib
Verify installation:

import matplotlib

print(matplotlib.__version__)
📦 Import Matplotlib
The most common import statement:

import matplotlib.pyplot as plt
pyplot provides functions for creating and customizing plots.

📊 Your First Plot
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [10, 20, 30, 40, 50]

plt.plot(x, y)
plt.show()
Output:

A simple line graph
📈 Line Plot
A line plot is used to show trends over time.

import matplotlib.pyplot as plt

months = ["Jan", "Feb", "Mar", "Apr"]
sales = [1000, 1200, 1500, 1800]

plt.plot(months, sales)

plt.title("Monthly Sales")
plt.xlabel("Month")
plt.ylabel("Sales")

plt.show()
Use Cases
Sales trends
Stock prices
Temperature changes
Website traffic
📊 Bar Chart
Used to compare categories.

import matplotlib.pyplot as plt

students = ["A", "B", "C", "D"]
marks = [80, 75, 90, 85]

plt.bar(students, marks)

plt.title("Student Marks")

plt.show()
Use Cases
Comparing products
Student performance
Department budgets
🥧 Pie Chart
Shows percentages and proportions.

import matplotlib.pyplot as plt

expenses = [40, 30, 20, 10]
labels = ["Food", "Rent", "Travel", "Other"]

plt.pie(
    expenses,
    labels=labels,
    autopct="%1.1f%%"
)

plt.show()
Use Cases
Budget allocation
Market share
Survey results
📉 Histogram
Shows data distribution.

import matplotlib.pyplot as plt

ages = [20,21,22,22,23,24,25,25,26,27]

plt.hist(ages, bins=5)

plt.title("Age Distribution")

plt.show()
Use Cases
Salary distribution
Exam scores
Customer ages
🔵 Scatter Plot
Shows relationships between two variables.

import matplotlib.pyplot as plt

hours = [1,2,3,4,5]
marks = [50,60,70,80,90]

plt.scatter(hours, marks)

plt.xlabel("Study Hours")
plt.ylabel("Marks")

plt.show()
Use Cases
Correlation analysis
Business analytics
Scientific experiments
🎨 Customizing Charts
Add Title
plt.title("Monthly Sales")
Add X-Axis Label
plt.xlabel("Month")
Add Y-Axis Label
plt.ylabel("Sales")
Add Grid
plt.grid(True)
Change Color
plt.plot(x, y, color="red")
Add Marker
plt.plot(x, y, marker="o")
Add Legend
plt.legend(["Sales"])
📐 Figure Size
Control plot size:

plt.figure(figsize=(8,5))
Example:

import matplotlib.pyplot as plt

plt.figure(figsize=(10, 6))

plt.plot(x, y)

plt.show()
🖼 Multiple Plots (Subplots)
Display multiple charts in one figure.

import matplotlib.pyplot as plt

plt.subplot(1, 2, 1)
plt.plot([1,2,3], [4,5,6])
plt.title("Plot 1")

plt.subplot(1, 2, 2)
plt.bar([1,2,3], [4,5,6])
plt.title("Plot 2")

plt.show()
💾 Save Charts
Save charts as image files.

plt.plot([1,2,3], [4,5,6])

plt.savefig("chart.png")
Supported formats:

PNG
JPG
PDF
SVG
Example:

plt.savefig("sales_report.pdf")
✅ Complete Example
import matplotlib.pyplot as plt

months = ["Jan", "Feb", "Mar", "Apr", "May"]
sales = [1000, 1200, 1500, 1800, 2100]

plt.figure(figsize=(8,5))

plt.plot(
    months,
    sales,
    color="blue",
    marker="o",
    linewidth=2
)

plt.title("Monthly Sales Trend")
plt.xlabel("Month")
plt.ylabel("Sales")
plt.grid(True)

plt.show()
🔑 Important Matplotlib Functions
Function	Purpose
plot()	Create line chart
bar()	Create bar chart
pie()	Create pie chart
hist()	Create histogram
scatter()	Create scatter plot
title()	Add title
xlabel()	Add X-axis label
ylabel()	Add Y-axis label
legend()	Add legend
grid()	Add grid
figure()	Set figure size
subplot()	Create multiple plots
savefig()	Save chart
show()	Display chart
💡 Best Practices
Use meaningful chart titles.
Label axes clearly.
Keep charts simple.
Avoid excessive colors.
Use legends when comparing data.
Select the right chart type.
Add grids for readability when needed.
Save important visualizations.
🌍 Real-World Applications
Business Dashboards
Sales Analysis
Marketing Reports
Financial Analytics
Healthcare Research
Scientific Studies
Machine Learning Projects
📝 Summary
Matplotlib is the most widely used Python visualization library. It provides tools for creating line charts, bar charts, histograms, scatter plots, pie charts, and more. Understanding Matplotlib is a fundamental step in learning Data Analysis, Data Science, and Machine Learning.

Key Takeaways
Matplotlib is the foundation of Python visualization.
Easy to create professional charts and graphs.
Supports extensive customization.
Works seamlessly with Pandas and NumPy.
Essential skill for every Data Analyst and Data Scientist.
Happy Learning! 🚀📊
