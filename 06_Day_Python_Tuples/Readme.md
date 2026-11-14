##📌 Introduction

A Tuple is a built-in Python data structure used to store multiple items in a single variable. Tuples are ordered, immutable (cannot be changed after creation), and allow duplicate values.

#Tuples are useful when you want to store data that should not be modified accidentally.

##🎯 Learning Objectives

By the end of this lesson, you will be able to:

- Understand what tuples are
- Create tuples in Python
- Access tuple elements
- Use tuple packing and unpacking
- Apply tuple methods
- Compare tuples and lists
- Use tuples in real-world scenarios

 ##📚 What is a Tuple?
A tuple is a collection of items enclosed in parentheses ().
fruits = ("apple", "banana", "mango")

print(fruits)
('apple', 'banana', 'mango')

## 🛠 Creating Tuples
Tuple with Multiple Values
colors = ("red", "green", "blue")
Mixed Data Types
mixed = (10, "Python", 3.14, True)
Empty Tuple
empty_tuple = ()

Single-Item Tuple

##⚠️ A comma is required when creating a tuple with one item.
fruit = ("apple",)

print(type(fruit))
🔍 Accessing Tuple Elements

Tuples use zero-based indexing.
fruits = ("apple", "banana", "mango")

print(fruits[0])
print(fruits[1])
print(fruits[-1])

apple
banana
mango
##✂️ Tuple Slicing
numbers = (10, 20, 30, 40, 50)

print(numbers[1:4])
(20, 30, 40)

##🔒 Tuple Immutability

Tuples cannot be modified after creation.
fruits = ("apple", "banana", "mango")

 This will produce an error
fruits[0] = "orange"
TypeError: 'tuple' object does not support item assignment
🎁 Tuple Packing

Packing means storing multiple values into a tuple.
person = ("John", 25, "Pune")

print(person)

##📦 Tuple Unpacking

Unpacking extracts tuple values into separate variables
person = ("John", 25, "Pune")

name, age, city = person

print(name)
print(age)
print(city)

John
25
Pune

## 🔄 Iterating Through Tuples
fruits = ("apple", "banana", "mango")

for fruit in fruits:
    print(fruit)
🛠 Tuple Methods

Tuples have only two built-in methods.

count()

Returns the number of times a value appears.
numbers = (1, 2, 2, 3, 2)

print(numbers.count(2))
3
index()

Returns the position of a value.
  numbers = (10, 20, 30, 40)

print(numbers.index(30))
2
## ⚖️ Lists vs Tuples
Feature	List	TupleSyntax	[]	()
Mutable	✅ Yes	❌ No
Ordered	✅ Yes	✅ Yes
Allows Duplicates	✅ Yes	✅ Yes
Performance	Slower	Faster
Methods	Many	Few

