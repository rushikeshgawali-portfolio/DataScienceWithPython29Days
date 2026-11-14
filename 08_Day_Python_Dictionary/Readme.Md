

## Overview
A dictionary in Python is a built-in data type used to store data in **key-value pairs**. Dictionaries are mutable, unordered (before Python 3.7), and allow fast data retrieval using keys.

## Learning Objectives
By the end of this lesson, you will be able to:

- Create and use dictionaries
- Access dictionary values
- Add, update, and remove items
- Loop through dictionary elements
- Use common dictionary methods
- Work with nested dictionaries

## Creating a Dictionary

```python
student = {
    "name": "John",
    "age": 21,
    "course": "Python"
}

print(student)
```

## Accessing Values

```python
print(student["name"])
print(student.get("age"))
```

## Adding Items

```python
student["city"] = "Mumbai"
print(student)
```

## Updating Items

```python
student["age"] = 22
print(student)
```

## Removing Items

### Using `pop()`

```python
student.pop("city")
```

### Using `del`

```python
del student["course"]
```

## Dictionary Methods

```python
student.keys()
student.values()
student.items()
student.clear()
```

## Looping Through a Dictionary

### Loop Through Keys

```python
for key in student:
    print(key)
```

### Loop Through Key-Value Pairs

```python
for key, value in student.items():
    print(key, value)
```

## Nested Dictionary Example

```python
employees = {
    "emp1": {
        "name": "Alice",
        "department": "HR"
    },
    "emp2": {
        "name": "Bob",
        "department": "IT"
    }
}

print(employees["emp1"]["name"])
```

## Example Program

```python
student = {
    "name": "Rahul",
    "age": 20,
    "marks": 85
}

for key, value in student.items():
    print(f"{key}: {value}")
```

## Key Points

- Dictionaries store data as key-value pairs.
- Keys must be unique.
- Values can be of any data type.
- Dictionaries are mutable.
- Useful for structured and real-world data storage.

## Practice Exercises

1. Create a dictionary to store employee information.
2. Add a new key-value pair to the dictionary.
3. Update an existing value.
4. Remove a key from the dictionary.
5. Display all keys and values using a loop.

## Conclusion

Dictionaries are one of the most powerful and commonly used data structures in Python. They provide an efficient way to organize, retrieve, and manipulate data using unique keys.
