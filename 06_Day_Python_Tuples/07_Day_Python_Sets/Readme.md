📌 Introduction

A Set is a built-in Python data structure used to store multiple unique items in a single variable.

Sets are:

✅ Unordered
✅ Mutable (can be modified)
✅ Do not allow duplicate values
✅ Useful for mathematical operations like union and intersection
🎯 Learning Objectives

By the end of this lesson, you will be able to:

Understand what sets are
Create and use sets in Python
Add and remove elements
Remove duplicates from data
Apply sets in real-world scenarios

📚 What is a Set?

A set is a collection of unique items enclosed in curly braces {}.
fruits = {"apple", "banana", "mango"}

print(fruits)
{'apple', 'banana', 'mango'}
🛠 Creating Sets
Set with Values
colors = {"red", "green", "blue"}
Mixed Data Types
mixed = {10, "Python", 3.14, True}
Empty Set

⚠️ Don't use {} because it creates a dictionary.
empty_set = set()

print(type(empty_set))
<class 'set'>
🔍 Accessing Set Elements

Sets are unordered, so indexing is not supported.

❌ Invalid:
fruits = {"apple", "banana", "mango"}

print(fruits[0])
TypeError: 'set' object is not subscriptable
for fruit in fruits:
    print(fruit)
➕ Adding Elements
add()

Adds a single item.
fruits = {"apple", "banana"}

fruits.add("mango")

print(fruits)
update()

Adds multiple items.
fruits = {"apple"}

fruits.update(["banana", "mango"])

print(fruits)
update()

Adds multiple items.
fruits = {"apple"}

fruits.update(["banana", "mango"])

print(fruits)

➖ Removing Elements
remove()

Removes a specific item.
fruits = {"apple", "banana", "mango"}

fruits.remove("banana")
print(fruits)

discard()

Removes an item if it exists.
fruits.discard("orange")

pop()
Removes a random item.
fruits.pop()

clear()

Removes all items.
fruits.clear()

🚫 Duplicate Values

Sets automatically remove duplicates.
numbers = {1, 2, 2, 3, 4, 4, 5}

print(numbers)
Output
{1, 2, 3, 4, 5}

🌎 Real-World Example

Remove duplicate email addresses.
emails = [
    "user1@gmail.com",
    "user2@gmail.com",
    "user1@gmail.com",
    "user3@gmail.com"
]

unique_emails = set(emails)

print(unique_emails)
 {'user1@gmail.com', 'user2@gmail.com', 'user3@gmail.com'}   
