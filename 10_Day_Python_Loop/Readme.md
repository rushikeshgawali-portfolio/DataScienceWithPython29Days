# 📘 Python Loops

Loops allow you to execute a block of code repeatedly, making your programs more efficient and easier to maintain.

## 🎯 Learning Objectives

After completing this lesson, you will be able to:

- Understand the purpose of loops
- Use `for` and `while` loops
- Control loop execution with `break` and `continue`
- Create nested loops
- Apply loops to real-world scenarios

---

## 🔄 What Is a Loop?

A **loop** repeats a block of code multiple times until a condition is met.

### Without a Loop

```python
print("Hello")
print("Hello")
print("Hello")
```

### With a Loop

```python
for i in range(3):
    print("Hello")
```

**Output**

```text
Hello
Hello
Hello
```

---

## 🔁 `for` Loop

Use a `for` loop when you want to iterate through a sequence or repeat an action a specific number of times.

### Syntax

```python
for item in sequence:
    # code block
```

### Example

```python
for number in range(5):
    print(number)
```

**Output**

```text
0
1
2
3
4
```

### Using `range()`

```python
range(5)       # 0 to 4
range(1, 6)    # 1 to 5
range(0, 11, 2)  # Even numbers from 0 to 10
```

---

## 📝 Looping Through a List

```python
fruits = ["Apple", "Banana", "Orange"]

for fruit in fruits:
    print(fruit)
```

**Output**

```text
Apple
Banana
Orange
```

---

## 🔁 `while` Loop

Use a `while` loop when you want to repeat code as long as a condition remains true.

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

**Output**

```text
1
2
3
4
5
```

> ⚠️ Always ensure the condition eventually becomes false to avoid infinite loops.

---

## ⛔ `break`

Stops the loop immediately.

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

**Output**

```text
0
1
2
3
4
```

---

## ⏭️ `continue`

Skips the current iteration and moves to the next one.

```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

**Output**

```text
0
1
3
4
```

---

## 🔄 Nested Loops

A nested loop is a loop inside another loop.

```python
for i in range(2):
    for j in range(3):
        print(i, j)
```

**Output**

```text
0 0
0 1
0 2
1 0
1 1
1 2
```

---

## 🌍 Real-World Example

Calculate the total price of items in a shopping cart.

```python
prices = [100, 200, 300]

total = 0

for price in prices:
    total += price

print(total)
```

**Output**

```text
600
```

---

## 🎭 Easy Analogies

### 🧺 Washing Machine

A washing machine repeats the same process for every load:

```text
Wash → Rinse → Spin
```

Loops repeat instructions in the same way.

### 👩‍🏫 Classroom Attendance

A teacher calls each student's name one at a time until everyone has been marked present.

A `for` loop works similarly by processing one item after another.

---

## ⚠️ Common Mistakes

### Infinite Loop

```python
while True:
    print("Hello")
```

### Forgetting to Update the Counter

```python
count = 1

while count <= 5:
    print(count)
```

✅ Correct:

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

---

## 📝 Practice Exercises

1. Print numbers from **1 to 10**.
2. Print all **even numbers** between **1 and 20**.
3. Find the **sum of numbers from 1 to 100**.
4. Print each character in `"Python"`.
5. Create a multiplication table for **5**.

---

## 🎯 Key Takeaways

- Loops automate repetitive tasks.
- `for` loops iterate through sequences.
- `while` loops run while a condition is true.
- `break` exits a loop immediately.
- `continue` skips the current iteration.
- Nested loops allow multi-level repetition.

