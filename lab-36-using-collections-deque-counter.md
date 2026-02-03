# Lab 36: Using Collections (deque, Counter)

## Lab Objectives
- Understand the `collections` module in Python, focusing on `deque` and `Counter`.
- Learn how to efficiently use a `deque` for appending and popping from both ends.
- Learn how to create and use a `Counter` for counting hashable objects.
- Analyze how these data structures improve performance and code clarity.

## Prerequisites
- Basic knowledge of Python programming.
- Familiarity with standard list and dictionary operations in Python.

---

## Task 1: Introduction to the collections Module

### Understanding the collections Module
The `collections` module is a built-in Python library that provides specialized container data types as alternatives to general-purpose containers like `list`, `dict`, and `tuple`.

Some commonly used data structures include:
- `deque`
- `Counter`
- `OrderedDict`
- `defaultdict`

These structures help write cleaner, more efficient, and more readable code.

---

## Task 2: Using deque

### Import deque from collections
```python
from collections import deque
Create and Manipulate a deque
Create a deque
d = deque()
Append elements to the deque
d.append('task1')
d.append('task2')
Pop from the right end
last_task = d.pop()
print("Popped from the right:", last_task)
Append to the left end
d.appendleft('task0')
Pop from the left end
first_task = d.popleft()
print("Popped from the left:", first_task)
Advantages of deque
Efficiency: Append and pop operations from both ends run in O(1) time.

Use Cases: Ideal for queues, stacks, browser history, task scheduling, and scenarios requiring fast access from both ends.

Task 3: Using Counter
Import Counter from collections
from collections import Counter
Create a Counter from a List of Words
Sample list of words
words = ['apple', 'orange', 'banana', 'apple', 'orange', 'apple']
Create a Counter object
word_count = Counter(words)
print("Word Count:", word_count)
Retrieve Most Common Elements
most_common = word_count.most_common(2)
print("Most Common Words:", most_common)
Advantages of Counter
Simplicity: Eliminates the need for manual counting using dictionaries.

Built-in Methods: Functions like most_common() make analysis easier and cleaner.

Readability: Produces concise and expressive code.

Conclusion
This lab explored the use of deque and Counter from Python’s collections module. These specialized data structures provide performance improvements and better code readability for common tasks like queue management and frequency counting. Understanding when and how to use them allows developers to write more efficient, maintainable, and Pythonic code.

