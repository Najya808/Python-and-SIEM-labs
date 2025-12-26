Lab 3: Data Types & Variables
🧠 What I Learned

In this lab, I learned how variables work in Python and how different data types are used to store information. I explored Python’s built-in data types, learned how to check variable types using the type() function, and understood the difference between implicit and explicit type casting. I also applied these concepts in a real-world case study involving customer data.

🎯 Lab Objectives

Understand variables and data types in Python

Create and manipulate different data types

Learn implicit and explicit type casting

Apply data type concepts in a practical scenario

🧪 Lab Tasks Performed
🔹 Task 1: Understanding and Creating Variables

Objective:
Learn how to create variables of different data types and check their types.

Step 1: Create Variables

Created variables of multiple data types in Python:

# Creating variables of different data types
name = "John Doe"      # String
age = 25               # Integer
is_student = True      # Boolean
height = 175.5         # Float

Step 2: Print Variables and Check Their Types

Used print() and type() to display values and data types:

print("Name:", name, "Type:", type(name))
print("Age:", age, "Type:", type(age))
print("Is Student:", is_student, "Type:", type(is_student))
print("Height:", height, "Type:", type(height))


Key Concept:
The type() function helps identify the data type stored in a variable.

🔹 Task 2: Implicit vs. Explicit Type Casting

Objective:
Understand how Python converts data types automatically and manually.

✅ Implicit Type Casting

Python automatically converts one data type to another when required.

a = 10      # Integer
b = 10.5    # Float

# Implicit casting from int to float
result = a + b
print("Result:", result, "Type:", type(result))


Observation:
The integer value was automatically converted to a float.

✅ Explicit Type Casting

The programmer manually converts data types using built-in functions.

# Integer to string
age_str = str(age)
print("Age as string:", age_str, "Type:", type(age_str))

# String to integer
number_str = "100"
number_int = int(number_str)
print("Number:", number_int, "Type:", type(number_int))


Key Concept:
Explicit casting gives full control over data conversion.

🔹 Task 3: Case Study – Customer Data Intake

Objective:
Apply variables and type casting to a real-world scenario.

Scenario

A system receives customer data as strings and needs proper data types for processing.

# Customer data
customer_name = "Alice Johnson"
customer_age = "30"          # Initially string
customer_membership = "True"

# Explicit casting
customer_age = int(customer_age)
customer_membership = customer_membership == "True"

print("Customer Name:", customer_name, "Type:", type(customer_name))
print("Customer Age:", customer_age, "Type:", type(customer_age))
print("Customer Membership Status:", customer_membership, "Type:", type(customer_membership))


Observation:
Explicit casting ensures data is stored in the correct format for logic and calculations.

Summary

In this lab, I successfully:

Created variables using different Python data types

Identified variable types using the type() function

Understood implicit and explicit type casting

Applied data type concepts in a practical case study

This lab strengthened my foundation in Python programming and prepared me for working with user input, conditions, and data processing in future labs.
