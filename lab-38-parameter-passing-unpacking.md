# Lab 38: Parameter Passing & Unpacking

## Objectives
- Understand the concept of parameter passing in Python.
- Explore the use of `*args` and `**kwargs` for function arguments.
- Learn how to unpack arguments using the `*` and `**` operators.
- Practice applying these concepts through hands-on tasks.

## Prerequisites
- Basic understanding of Python functions and data types.
- Familiarity with lists and dictionaries in Python.

---

## Task 1: Using `*args` to Sum an Arbitrary Number of Arguments

### Introduction to `*args`
- `*args` allows you to pass a variable number of arguments to a function.
- The arguments are stored as a tuple inside the function.

### Example
```python
def sum_numbers(*args):
    return sum(args)
Exercise
Write a function add_numbers using *args to calculate the sum of all arguments passed.

def add_numbers(*args):
    total = 0
    for num in args:
        total += num
    return total
Test Case
print(add_numbers(1, 2, 3, 4, 5))  # Output: 15
Task 2: Using **kwargs to Print Named Parameters
Introduction to **kwargs
**kwargs allows you to pass a variable number of keyword arguments.

The arguments are stored as a dictionary inside the function.

Example
def print_kwargs(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")
Exercise
Write a function show_info using **kwargs to print named parameters and their values.

def show_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")
Test Case
show_info(name="Alice", age=30, city="New York")
Task 3: Unpacking Arguments Using * and **
Unpacking with *
The * operator can unpack a list or tuple into positional arguments.

numbers = [1, 2, 3, 4]
print(sum_numbers(*numbers))
Unpacking with **
The ** operator can unpack a dictionary into keyword arguments.

data = {'name': 'John', 'age': 25}
print_kwargs(**data)
Exercise
Create a dictionary and unpack it into the show_info function.

info = {'occupation': 'Engineer', 'country': 'USA'}
show_info(**info)
Conclusion
In this lab, we explored flexible parameter passing in Python using *args and **kwargs.
We also practiced unpacking lists and dictionaries using * and ** operators.
These techniques are essential for writing reusable, scalable, and clean Python functions that can handle varying input sizes efficiently.
