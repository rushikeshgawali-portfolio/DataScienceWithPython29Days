Day 05: Python Lists
📌 Introduction

A List is one of the most commonly used data structures in Python. Lists allow you to store multiple items in a single variable and are ordered, mutable, and can contain different data types.

🎯 Learning Objectives

By the end of this lesson, you will be able to:

Create Python lists
Access list elements
Modify list items
Add and remove elements
Slice lists
Use common list methods
Iterate through lists
Perform basic list operations

📚Creating a List
# Empty list
my_list = []

# List with values
fruits = ["apple", "banana", "mango"]

# Mixed data types
mixed = [10, "Python", 3.14, True]
🔍 Accessing Elements

Lists use zero-based indexing.
fruits = ["apple", "banana", "mango"]

print(fruits[0])   # apple
print(fruits[1])   # banana
print(fruits[-1])  # mango

✏️ Modifying List Elements
fruits = ["apple", "banana", "mango"]

fruits[1] = "orange"

print(fruits)
# Output: ['apple', 'orange', 'mango']

➕ Adding Elements
append()
fruits = ["apple", "banana"]
fruits.append("mango")

print(fruits)

insert()
fruits.insert(1, "orange")

print(fruits)
➖ Removing Elements
remove()
fruits.remove("banana")
pop()
fruits.pop()
delete
del fruits[0]
✂️ List Slicing
numbers = [1, 2, 3, 4, 5, 6]

print(numbers[1:4])
# Output: [2, 3, 4]
🔄 Looping Through Lists
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)


🛠 Common List Methods
Method	Descriptionappend()	Adds an item to the end
insert()	Inserts an item at a specific position
remove()	Removes a specific item
pop()	Removes and returns an item
sort()	Sorts the list
reverse()	Reverses the list
count()	Counts occurrences of an item
index()	Returns the index of an item
clear()	Removes all items

📊 Example Program
students = ["John", "Alice", "Bob"]

students.append("David")

for student in students:
    print(student)

print("Total Students:", len(students))

John
Alice
Bob
David
Total Students: 4

📝 Practice Exercises
Create a list of your favorite movies.
Add a new movie to the list.
Remove one movie from the list.
Print the first and last movie.
Sort the list alphabetically.
Count the total number of movies.
✅ Key Takeaways
Lists are ordered and mutable collections.
Indexing starts from 0.
Use append() and insert() to add items.
Use remove(), pop(), and del to delete items.
Lists support slicing and iteration.
Many built-in methods make list manipulation easy.

