Lab 2: Hello World & Basic Syntax
What I Learned

In this lab, I learned how to create and execute a simple Python script using the command line. I also understood Python’s basic syntax rules, especially how indentation is used to define code blocks. Through experimentation, I observed how incorrect indentation leads to errors, reinforcing the importance of proper formatting in Python.

🎯 Lab Objectives

Create a simple Python script

Execute a Python script using the command line

Understand Python’s indentation-based syntax

Experiment with basic control structures

🧪 Lab Tasks Performed

🔹 Task 1: Create a Simple Python Script
Step 1: Open a Text Editor

Opened a text editor such as Visual Studio Code or Notepad++

Created a new file named:

hello.py

Step 2: Write a Python Script

Added the following code to hello.py:

print("Hello, World!")


Key Concept:
Python scripts are saved with the .py extension and executed using the Python interpreter.

🔹 Task 2: Run the Python Script
Step 1: Open the Command Line Interface

Windows: Command Prompt or PowerShell

macOS/Linux: Terminal

Step 2: Navigate to the File Directory

Used the cd command to move to the directory containing hello.py:

cd Documents

Step 3: Execute the Script

Ran the script using:

python hello.py


Output:

Hello, World!


Observation:
The script executed successfully and printed output to the console.

🔹 Task 3: Experiment with Indentation
Step 1: Modify the Script

Updated hello.py with a simple if statement:

if True:
    print("This will always print because the condition is True.")
print("Hello, World!")

Step 2: Understand Indentation

The indented line belongs to the if block

Python uses indentation instead of braces {} to define code blocks

Step 3: Test Incorrect Indentation

Modified the script incorrectly:

if True:
print("This will cause an IndentationError.")


Result:
Python raised an IndentationError.

Step 4: Fix the Error

Corrected the indentation:

if True:
    print("This will always print because the condition is True.")


Key Concept:
Consistent indentation is mandatory in Python and is part of the language syntax.

Summary

In this lab, I successfully:

Created and executed my first Python script

Learned how Python programs are run from the command line

Understood Python’s indentation-based structure

Observed and fixed indentation-related syntax errors

This lab strengthened my understanding of Python fundamentals and prepared me for writing structured and logical Python programs.
