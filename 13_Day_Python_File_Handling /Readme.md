## Introduction

Files allow programs to store data permanently. Without files, any data created by a program is lost when the program stops running.

File Handling in Python is the process of creating, reading, writing, and modifying files. It enables programs to save information such as user data, reports, logs, and application settings.

Real-Life Analogy

Imagine a notebook:

Write → Add information to the notebook.
Read → View information from the notebook.
Update → Modify existing information.
Delete → Remove information.

A file works the same way in Python.

Why File Handling is Important

File handling allows you to:

✅ Store data permanently

✅ Read existing data

✅ Update information

✅ Create reports and logs

✅ Work with text and data files

✅ Build real-world applications

What is a File?

A file is a collection of data stored on a computer.

Examples:

Plain Text
notes.txt
students.csv
data.json
report.pdf

Python can interact with many types of files, but beginners usually start with text files (.txt).

Opening a File

Python uses the open() function to open a file.

Syntax
Python
open(filename, mode)

Example:

Python
file = open("sample.txt", "r")

Here:

"sample.txt" → File name
"r" → Read mode
File Modes
Mode	Description
r	Read file
w	Write file (overwrite existing content)
a	Append data to file
x	Create a new file
r+	Read and write
Reading Files
Read Entire File
Python
file = open("sample.txt", "r")
 
content = file.read()
 
print(content)
 
file.close()

Example Output:

Plain Text
Hello Python
Welcome to File Handling
Read One Line
Python
file = open("sample.txt", "r")
 
print(file.readline())
 
file.close()

Output:

Plain Text
Hello Python
Read All Lines
Python
file = open("sample.txt", "r")
 
for line in file:
print(line)
 
file.close()
Writing to a File

The w mode creates a file if it does not exist and overwrites existing content.

Python
file = open("sample.txt", "w")
 
file.write("Hello Python")
 
file.close()

Result:

Plain Text
sample.txt
-----------
Hello Python

⚠️ Existing content will be removed.

Appending Data

The a mode adds content without removing existing content.

Python
file = open("sample.txt", "a")
 
file.write("\nLearning File Handling")
 
file.close()

Result:

Plain Text
Hello Python
Learning File Handling
Closing a File

Always close files after use.

Python
file = open("sample.txt", "r")
 
print(file.read())
 
file.close()

Closing files:

Frees system resources
Prevents data loss
Improves performance
Using with Statement

A better way to work with files is using with.

Python automatically closes the file when the block finishes.

Python
with open("sample.txt", "r") as file:
content = file.read()
print(content)

✅ Recommended approach

✅ Cleaner code

✅ Automatically closes files

Creating a New File
Python
file = open("new_file.txt", "w")
 
file.write("This is a new file.")
 
file.close()

Python creates the file if it doesn't already exist.

Checking if a File Exists
Python
import os
 
if os.path.exists("sample.txt"):
print("File exists")
else:
print("File not found")
Mini Project: Notes Saver
Python
note = input("Enter a note: ")
 
with open("notes.txt", "a") as file:
file.write(note + "\n")
 
print("Note saved successfully!")

Example:

Plain Text
Enter a note: Learn Python daily
Note saved successfully!

Stored in:

Plain Text
notes.txt
-----------
Learn Python daily
Beginner Practice Exercises
Exercise 1

Create a file named message.txt and write:

Plain Text
Hello World
Exercise 2

Read and display the contents of message.txt.

Exercise 3

Append the text:

Plain Text
Python is fun!

to the file.

Exercise 4

Use the with statement to read a file.

Exercise 5

Create a simple program that stores three user names in a text file.

Common Mistakes
Forgetting to Close a File
Python
file = open("sample.txt", "r")
print(file.read())

Better:

Python
with open("sample.txt", "r") as file:
print(file.read())
Using Write Mode Accidentally
Python
open("data.txt", "w")

This removes existing content.

Use append mode when you want to keep old data:

Python
open("data.txt", "a")
Key Takeaways

✅ File handling allows programs to store data permanently.

✅ Use open() to open files.

✅ Use read() to read file contents.

✅ Use write() to write data.

✅ Use append (a) mode to add new content.

✅ Always close files or use the with statement.

✅ Text files (.txt) are the most common starting point for beginners.

Memory Trick

📒 File = Notebook

Read → View notes
Write → Replace notes
Append → Add more notes
Close → Put the notebook away safely

File Handling = Managing your digital notebook with Python. 🐍📂

Add exception handling examplesInclude CSV and JSON filesCreate a file-handling mini project
AllTabsTabsFilesFiles
