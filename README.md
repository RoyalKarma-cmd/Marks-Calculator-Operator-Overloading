# Marks Calculator using Operator Overloading

## Project Overview

This project demonstrates **Operator Overloading** in Python using the special (dunder) method:

```python
__add__()
```

The project allows two custom `Marks` objects to be added together using the `+` operator, just like built-in data types.

This project was developed as part of my Python Object-Oriented Programming (OOP) learning journey.

---

## Features

- Store marks using custom objects
- Add marks using the `+` operator
- Understand Python's special methods
- Learn Operator Overloading
- Explore the internal working of Python operators

---

## Concepts Used

### Classes and Objects

A custom class named `Marks` is used to store marks.

```python
class Marks:
```

---

### Constructor

The constructor initializes the marks value.

```python
def __init__(self, marks):
    self.marks = marks
```

---

### Operator Overloading

The `__add__()` method customizes the behavior of the `+` operator.

```python
def __add__(self, other):
    return self.marks + other.marks
```

When Python sees:

```python
science + history
```

it internally executes:

```python
science.__add__(history)
```

---

## Code Example

```python
class Marks:

    def __init__(self, marks):
        self.marks = marks

    def __add__(self, other):
        return self.marks + other.marks


science = Marks(75)
history = Marks(55)

print(science + history)
```

---

## Sample Output

```text
130
```

---

## How It Works

### Step 1

Create two objects:

```python
science = Marks(75)
history = Marks(55)
```

### Step 2

Use the `+` operator:

```python
science + history
```

### Step 3

Python calls:

```python
science.__add__(history)
```

### Step 4

The method returns:

```python
75 + 55
```

### Step 5

Output:

```text
130
```

---

## OOP Concepts Demonstrated

- Classes
- Objects
- Constructors
- Methods
- Dunder Methods
- Operator Overloading

---

## Learning Outcomes

Through this project, I learned:

- How Python operators work internally
- The purpose of special methods (dunder methods)
- Operator Overloading using `__add__()`
- Creating custom behavior for objects
- Object-Oriented Programming concepts

---

## Future Improvements

- Multiple Subject Support
- Percentage Calculator
- Grade Calculator
- Student Result Management System
- GPA Calculator

---

## Technologies Used

- Python
- Object-Oriented Programming (OOP)

---

## Repository Structure

marks-calculator-operator-overloading/
│
├── marks_calculator.py
├── README.md
└── practice-notebook/

---

## Author

**Jaydeep**

Day 14 Project – Marks Calculator using Operator Overloading

Part of my 1-Year Data Science & Machine Learning Roadmap 🚀
