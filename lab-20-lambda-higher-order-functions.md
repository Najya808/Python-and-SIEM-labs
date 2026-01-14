What I Learned

In this lab, I learned how to create lambda functions, which are anonymous, inline functions in Python. I also explored higher-order functions such as map(), filter(), and reduce() to perform operations on data collections. This lab helped me understand how to write concise, functional-style code to process lists efficiently and improve readability.

Lab Objectives

Understand lambda functions and their syntax

Use higher-order functions: map, filter, reduce

Implement practical tasks using lambda and higher-order functions

Learn benefits of concise, readable functional programming in Python

📋 Prerequisites

Basic Python programming knowledge

Familiarity with lists and list operations

Python development environment (IDE or Jupyter Notebook)

🧪 Lab Tasks Performed

🔹 Task 1: Creating a List of Numbers

# Define a list of numbers
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]


Explanation: Initialized a list of integers from 1 to 10 for testing higher-order functions.

🔹 Task 2: Doubling Numbers Using map and Lambda

# Use map with a lambda function to double the numbers
doubled_numbers = list(map(lambda x: x * 2, numbers))
print("Doubled Numbers:", doubled_numbers)


Key Concept:

Lambda function: lambda x: x * 2 is an anonymous function that doubles a number

Map function: Applies the lambda to each item in the list

🔹 Task 3: Filtering Even Numbers Using filter and Lambda

# Use filter with a lambda function to select even numbers
even_numbers = list(filter(lambda x: x % 2 == 0, numbers))
print("Even Numbers:", even_numbers)


Key Concept:

filter() returns items for which the lambda function evaluates to True

Here, only even numbers are retained

🔹 Task 4: Reducing the List to a Sum Using reduce

from functools import reduce

# Use reduce with a lambda function to sum the numbers
total_sum = reduce(lambda x, y: x + y, numbers)
print("Sum of Numbers:", total_sum)


Key Concept:

reduce() applies a function cumulatively to the items of a list

Here, the lambda function adds elements from left to right to produce a single sum

🧩 Key Concepts Covered

Lambda functions for anonymous, inline operations

map() for transforming each element in a collection

filter() for selecting elements based on a condition

reduce() for collapsing a collection into a single value

Functional programming concepts for concise and readable Python code

Conclusion

In this lab, I successfully:

Created and used lambda functions

Applied map, filter, and reduce with lambda functions

Learned the benefits of functional programming for concise and readable code

Practiced higher-order functions to perform data processing efficiently

Benefits Highlighted:

Lambda functions create quick, one-line functions without naming them

Higher-order functions with lambda lead to cleaner, readable, and more Pythonic code

Functional programming is useful in tasks like data processing, transformations, and aggregations
