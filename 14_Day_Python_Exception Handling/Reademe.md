# Python Exception Handling

## Introduction

While running a program, errors can occur due to invalid input, missing files, incorrect calculations, or unexpected situations. If these errors are not handled properly, the program may stop abruptly.

**Exception Handling** allows us to catch and manage errors so that the program can continue running smoothly.

### Real-Life Analogy

Imagine you're driving a car and encounter a roadblock.

- Without exception handling → Your journey stops immediately.
- With exception handling → You take a different route and continue.

Similarly, Python uses exception handling to deal with unexpected errors without crashing the program.

---

## What is an Exception?

An **exception** is an error that occurs while a program is running.

### Example

```python
print(10 / 0)
```

### Output

```text
ZeroDivisionError: division by zero
```

Python stops execution because dividing by zero is not allowed.

---

## Why Exception Handling is Important

✅ Prevents program crashes

✅ Improves user experience

✅ Makes programs more reliable

✅ Helps identify and manage errors

✅ Allows programs to continue running

---

## The `try` and `except` Blocks

The basic structure of exception handling is:

```python
