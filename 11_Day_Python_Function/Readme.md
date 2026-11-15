# 📘  Python Functions

Functions help you organize and reuse code by grouping instructions into a single, reusable block.

## 🎯 Learning Objectives

- Create and call functions
- Pass arguments to functions
- Return values
- Use default parameters
- Understand variable scope



## 💡 What Is a Function?

A **function** is a reusable block of code that performs a specific task.

python
def greet():
    print("Hello, World!")

greet()


**Output**

text
Hello, World!




## 🔨 Creating a Function

Use the `def` keyword to define a function.

python
def welcome():
    print("Welcome to Python!")

welcome()


## 📥 Parameters

Parameters allow you to pass data into a function.

python
def greet(name):
    print(f"Hello, {name}!")

greet("John")


**Output**

text
Hello, John!


## 📤 Return Values

Use `return` to send data back.

python
def add(a, b):
    return a + b

print(add(5, 3))


**Output**

text
8


## ⚙️ Default Parameters

Provide a default value if no argument is passed.

python
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()


**Output**
text
Hello, Guest!

## 🌍 Real-World Example

python
def calculate_area(length, width):
    return length * width

print(calculate_area(10, 5))


**Output**

text
50




## 🎭 Easy Analogies

### ☕ Coffee Machine

text
Ingredients → Brew
