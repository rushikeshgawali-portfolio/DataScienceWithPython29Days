## 🌳 Decision Tree with Python Example

A beginner-friendly example showing how a Decision Tree predicts whether a student will Pass or Fail.

## 📊 Dataset
Study Hours	Result
2	Fail
3	Fail
5	Pass
7	Pass
🌳 Decision Tree Diagram
Plain Text
[Study Hours > 4?]
│
┌─────────┴─────────┐
│ │
No Yes
│ │
▼ ▼
[Fail ❌] [Pass ✅]
## 🐍 Python Code
Python
from sklearn.tree import DecisionTreeClassifier
 
# Training Data
X = [[2], [3], [5], [7]] # Study Hours
y = ["Fail", "Fail", "Pass", "Pass"]
 
# Create and Train Model
model = DecisionTreeClassifier()
model.fit(X, y)
 
# Predict for a student who studied 6 hours
prediction = model.predict([[6]])
 
print("Prediction:", prediction[0])
Output
Plain Text
Prediction: Pass
## 🔍 Code Explanation
1. Import Decision Tree
Python
from sklearn.tree import DecisionTreeClassifier

Imports the Decision Tree algorithm.

2. Create Training Data
Python
X = [[2], [3], [5], [7]]
y = ["Fail", "Fail", "Pass", "Pass"]
X = Study Hours (Input)
y = Result (Output)
3. Train the Model
Python
model.fit(X, y)

The model learns the relationship between study hours and results.

4. Make a Prediction
Python
model.predict([[6]])

Asks:

"A student studied 6 hours. Will they Pass or Fail?"

The model predicts:

Plain Text
Pass ✅
## 🎯 Real-Life Analogy

Imagine a teacher says:

Plain Text
If Study Hours > 4
↓
Pass
 
Else
↓
Fail

A Decision Tree learns and creates these rules automatically from data.

## 🚀 Quick Revision
Plain Text
Decision Tree = Questions → Answers → Decision
 
Python Steps:
1. Import DecisionTreeClassifier
2. Create Data
3. Train Model
4. Predict Result
 
Example:
Study Hours → Pass/Fail
One-Line Definition

A Decision Tree is a Machine Learning algorithm that learns rules from data and makes predictions by asking simple questions. 🌳
