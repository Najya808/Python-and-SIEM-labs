What I Learned

In this lab, I learned how to make Python programs more robust by handling errors and unexpected inputs using exception handling. I practiced using try, except, and finally blocks to catch errors gracefully, and learned how to differentiate between multiple types of exceptions. This helps prevent program crashes and allows for appropriate responses to user input or runtime issues.

🎯 Lab Objectives

Understand the fundamentals of exception handling in programming

Learn to use try, except, and finally blocks to manage errors

Practice implementing exception handling in Python

Identify different types of exceptions and handle them efficiently

🧪 Lab Tasks Performed

🔹 Task 1: Prompt User for Input

Objective: Capture user input and prepare for exception handling.

# Prompt the user for input
user_input = input("Enter a number: ")


Explanation:

The input() function is used to capture user input.

This input may later trigger exceptions if it cannot be converted or used in calculations.

🔹 Task 2: Convert Input to Integer with Exception Handling

Objective: Safely convert user input to an integer.

try:
    number = int(user_input)
    print(f"The number is {number}.")
except ValueError as ve:
    print("Error: Input is not a valid number. Please enter an integer.")


Explanation:

try block: Contains code that might raise an exception.

except block: Executes if an exception occurs, preventing program crash.

ValueError handles cases where input cannot be converted to an integer.

🔹 Task 3: Implement Multiple Except Blocks

Objective: Differentiate and handle multiple exceptions.

try:
    result = 10 / int(user_input)
    print(f"Result is: {result}")
except ValueError:
    print("Error: Please enter numeric values!")
except ZeroDivisionError:
    print("Error: Division by zero is undefined!")


Explanation:

Multiple except blocks allow handling of different exception types separately.

ValueError manages invalid numeric input.

ZeroDivisionError manages division by zero errors.

🧩 Key Concepts

Exception handling: Process of responding to runtime errors in a controlled way.

try block: Code that might cause an exception.

except block: Code executed when an exception occurs.

Multiple except blocks: Manage different exception types separately.

finally block (optional): Executes code regardless of whether an exception occurred, often used for cleanup.

Summary

Handled user input safely using try and except.

Learned to differentiate between different exception types.

Gained practical experience in creating robust, crash-resistant programs.

Prepared for real-world scenarios where input or operations may fail.
