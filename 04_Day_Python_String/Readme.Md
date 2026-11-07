# Welcome to Day 4 of the 29-Day Data Science with Python journey! Today's focus is on mastering Strings—one of the most commonly used data types in data preprocessing and text analysis.
​📝 Topics Covered
​String Creation & Indexing: Accessing individual characters and substrings.
​String Slicing: Extracting specific portions of text using [start:end:step].
​Built-in String Methods: Cleaning and manipulating text using methods like .lower(), .upper(), .strip(), .replace(), and .split().
​String Formatting: Using f-strings (f"...") for clean variable interpolation.
​💻 Code Examples
​1. Slicing and Indexing
text = "DataScience"
print(text[0:4])  # Output: Data
print(text[-7:])  # Output: Science

common string methood
messy_text = "   Hello, Data Analyst!   "
print(messy_text.strip().lower())  # Output: hello, data analyst!
print(messy_text.replace("Analyst", "Scientist"))

🚀 Key Takeaways
​Strings are immutable in Python, meaning once created, they cannot be changed in place.
​Text preprocessing is a crucial first step in Natural Language Processing (NLP) and general data cleaning pipelines.
