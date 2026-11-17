## Introduction

As programs become larger, managing everything with variables and functions can become difficult. Object-Oriented Programming (OOP) helps organize code by grouping related data and actions together.

Don't worry if the term sounds complicated.

Think of OOP as a way to describe real-world things in Python.

For example:

A Car has a color, model, and speed.
A Student has a name, age, and grade.
A Bank Account has an account number and balance.

In Python, we can create these real-world objects using OOP.

Why Learn OOP?

OOP helps you:

✅ Organize code better

✅ Reuse code easily

✅ Build real-world applications

✅ Reduce repetition

✅ Make programs easier to maintain

Real-Life Analogy

Imagine you're filling out a college admission form.

Every student has:

Name
Age
Course

And every student can:

Study
Attend classes
Take exams

Similarly in Python:

Data → Attributes
Actions → Methods

Together they form an Object.

What is an Object?

An Object is a real-world thing that contains data and actions.

Example

A mobile phone:

Data (Attributes)

Brand
Model
Price

Actions (Methods)

Call
Send Message
Take Photo

In Python, we represent this using a class.

What is a Class?

A Class is a blueprint or template used to create objects.

Real-Life Example

Think of a house blueprint.

The blueprint is not a house.

Using the blueprint, many houses can be built.

Similarly:

Class = Blueprint
Object = Actual House
Creating a Simple Class
Python
class Student:
pass

This creates an empty class called Student.

Creating an Object
Python
class Student:
pass
 
student1 = Student()
 
print(student1)

Output:

Plain Text
<__main__.Student object at 0x...>

Here:

Student is the class.
student1 is an object.
The __init__() Method

The __init__() method automatically runs when an object is created.

It is used to assign values to an object.

Python
class Student:
def __init__(self, name, age):
self.name = name
self.age = age
 
student1 = Student("Rahul", 20)
 
print(student1.name)
print(student1.age)

Output:

Plain Text
Rahul
20
Understanding self

self refers to the current object.

Think of it as saying:

"My name" or "My age"

Example:

Python
class Student:
def __init__(self, name):
self.name = name

When an object is created:

Python
student1 = Student("Rahul")

Python stores:

Plain Text
student1.name = Rahul
Methods in Classes

Methods are functions inside a class.

Python
class Student:
def __init__(self, name):
self.name = name
 
def greet(self):
print("Hello, my name is", self.name)
 
student1 = Student("Rahul")
 
student1.greet()

Output:

Plain Text
Hello, my name is Rahul
 
Creating Multiple Objects

One class can create multiple objects.

Python
class Student:
def __init__(self, name):
self.name = name
 
student1 = Student("Rahul")
student2 = Student("Priya")
 
print(student1.name)
print(student2.name)

Output:

Plain Text
Rahul
Priya
 
OOP Concepts

Python OOP has four important concepts:

Encapsulation
Inheritance
Polymorphism
Abstraction

Let's understand them with simple examples.

1. Encapsulation

Encapsulation means keeping related data and methods together inside a class.

Real-Life Example

A bank account contains:

Balance
Account Number

Operations:

Deposit
Withdraw

Everything is kept together.

Python
class BankAccount:
def __init__(self, balance):
self.balance = balance
 
def deposit(self, amount):
self.balance += amount
 
account = BankAccount(1000)
 
account.deposit(500)
 
print(account.balance)

Output:

Plain Text
1500
2. Inheritance

Inheritance allows one class to use features of another class.

Real-Life Example

A dog is an animal.

A cat is also an animal.

Both can inherit common characteristics from the Animal class.

Python
class Animal:
def eat(self):
print("Eating")
 
class Dog(Animal):
pass
 
dog = Dog()
 
dog.eat()

Output:

Plain Text
Eating
3. Polymorphism

Polymorphism means one action can behave differently for different objects.

Real-Life Example

Different vehicles make different sounds.

Python
class Dog:
def sound(self):
print("Bark")
 
class Cat:
def sound(self):
print("Meow")
 
dog = Dog()
cat = Cat()
 
dog.sound()
cat.sound()

Output:

Plain Text
Bark
Meow

Same method name, different behavior.

4. Abstraction

Abstraction means hiding unnecessary details and showing only what is important.

Real-Life Example

You drive a car by:

Starting it
Steering it
Accelerating

You don't need to know how the engine works internally.

In programming, abstraction hides complexity from users.

Mini Project: Employee Information System
Python
class Employee:
def __init__(self, name, department):
self.name = name
self.department = department
 
def display(self):
print("Name:", self.name)
print("Department:", self.department)
 
employee1 = Employee("Rahul", "HR")
 
employee1.display()

Output:

Plain Text
Name: Rahul
Department: HR
Best Practices
✅ Use Meaningful Class Names

Good:

Python
class Student:
pass

Bad:

Python
class S:
pass
✅ Use Meaningful Method Names

Good:

Python
def calculate_total():
pass

Bad:

Python
def xyz():
pass
 
✅ One Class, One Responsibility

Good:

Python
class Student:
pass
Python
class Teacher:
pass

Avoid putting everything into one class.

✅ Keep Classes Simple

Start with small classes and add features gradually.

✅ Reuse Code Through Inheritance

Instead of copying code, inherit from existing classes when appropriate.

Beginner Practice Exercises
Exercise 1

Create a class called Car.

Store:

Brand
Model

Create an object and display the values.

Exercise 2

Create a class called Employee.

Store:

Name
Salary

Print employee details.

Exercise 3

Create a class called BankAccount.

Add:

Balance
Deposit Method
Exercise 4

Create an Animal class and a Dog class using inheritance.

Exercise 5

Create two classes:

Dog
Cat

Add a sound() method to each class.

Common Mistakes
❌ Forgetting self

Wrong:

Python
class Student:
def greet():
print("Hello")

Correct:

Python
class Student:
def greet(self):
print("Hello")
❌ Creating Objects Without Required Values

Wrong:

Python
student = Student()

If the constructor expects values.

Correct:

Python
student = Student("Rahul", 20)
Summary
OOP stands for Object-Oriented Programming.
A Class is a blueprint.
An Object is an instance of a class.
__init__() initializes object data.
self refers to the current object.
Methods are functions inside classes.
The four main OOP concepts are:
Encapsulation
Inheritance
Polymorphism
Abstraction
Memory Trick

🏠 Class = House Blueprint

🏠 Object = Actual House

👤 Attributes = Information about the house (color, size, rooms)

🚪 Methods = Actions (open door, switch on lights)

If you understand the difference between a blueprint and a real house, you've already understood the foundation of Python OOP! 🚀🐍
