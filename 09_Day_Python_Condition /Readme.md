## 📖 Introduction

In our daily life, we make decisions based on conditions.

For example:

If it is raining, take an umbrella.
If your exam score is above 50, you pass.
If your phone battery is low, charge it.

Python works in a similar way. It uses conditions to decide what action to perform.

Conditions help a program think and make decisions based on different situations.
## 🎯 Learning Objectives

By the end of this lesson, you will be able to:

✅ Understand decision-making in Python
 ✅ Use if statements
 ✅ Use if...else statements
 ✅ Use if...elif...else statements
 ✅ Compare values using comparison operators
 ✅ Build simple real-world programs
## 🤔 What is a Condition?

A condition is a question that can have only two answers:
True
False
## Example
age = 20

print(age >= 18)
Output
True

Here Python checks:

Is age greater than or equal to 18?

Answer: True
## 🔹 The if Statement

The if statement executes code only when a condition is true.

Syntax
Python
if condition:
# Code to execute

#Example
age = 20

if age >= 18:
    print("You can vote.")
  ## Output
   You can vote.

  ## 🌍 Real-Life Example

Imagine a movie theatre.

Python
age = 15
 
if age >= 13:
print("You can watch this movie.")

Since age is 15, the message will be displayed.

##🔹 The if...else Statement

Sometimes there are only two possible outcomes.

Example
Python
age = 16
 
if age >= 18:
print("You can vote.")
else:
print("You cannot vote yet.")

Output
Python
You cannot vote yet.
How It Works
If condition is true → execute if block
Otherwise → execute else block

## 3. if...elif...else Statement

Used when multiple conditions need to be checked.

Python
marks = 75
 
if marks >= 90:
print("Grade A")
elif marks >= 70:
print("Grade B")
else:
print("Grade C")

Output:

Grade B

## Comparison Operators

These operators help compare values.

Operator	Meaning	Example
==	Equal to	x == y
!=	Not equal to	x != y
>	Greater than	x > y
	Less than	x < y
>=	Greater than or equal to	x >= y
<=	Less than or equal to	x <= y
## Logical Operators

Used to combine multiple conditions.

and

Returns True if all conditions are True.

Python
age = 25
has_license = True
 
if age >= 18 and has_license:
print("You can drive")
or

Returns True if at least one condition is True.

Python
if age < 18 or has_license:
print("Condition met")
not

Reverses the condition.

Python
is_raining = False
 
if not is_raining:
print("Go outside")
Nested Conditions

You can place one condition inside another.

Python
age = 20
has_id = True
 
if age >= 18:
if has_id:
print("Entry allowed")
Real-World Example
Python
temperature = 32
 
if temperature > 35:
print("It's very hot")
elif temperature > 25:
print("Nice weather")
else:
print("It's cool")
## Key Points to Remember

✅ Use if for a single condition.
 ✅ Use if...else for two possible outcomes.
 ✅ Use if...elif...else for multiple decision paths.
 ✅ Conditions evaluate to either True or False.
 ✅ Indentation is important in Python and defines the code block.
