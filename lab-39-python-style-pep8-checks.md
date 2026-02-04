# Lab 39: Python Style & PEP 8 Checks

## Objectives
- Understand the importance of Python style guides, focusing on PEP 8.
- Learn how to check Python code for style consistency using flake8.
- Practice improving code readability and styling through automated formatting tools like black and autopep8.

## Prerequisites
- Basic knowledge of Python programming.
- Python and pip installed on your system.

## Introduction
PEP 8 is the official style guide for Python code. It defines conventions for writing readable, consistent, and maintainable Python programs. Following PEP 8 is especially important in collaborative projects.  
Tools such as **flake8**, **black**, and **autopep8** help developers automatically detect and fix style issues efficiently.

---

## Lab Tasks

### Task 1: Install flake8
Open your terminal or command prompt and install flake8 using pip:

```bash
pip install flake8
Note: flake8 checks Python code for syntax errors, logical issues, and PEP 8 style violations.

Task 2: Run flake8 on a Sample Script
Create a Python file named example.py with intentional PEP 8 violations:

def exampleFunction():
    x = { 'key' : 42 , 'another_key': 23 }

    if(x['key'] >0): print("Positive number")

    else:print("Zero or Negative")
Run flake8 on the file:

flake8 example.py
Observations
Common issues reported by flake8 may include:

Improper function naming (should be lowercase with underscores).

Extra spaces inside brackets.

Missing spaces around operators.

Multiple statements on a single line.

Document the warnings or errors reported by flake8.

Task 3: Format Code Using black
Install black:

pip install black
Format the file using black:

black example.py
Observation
Black automatically reformats the code to match PEP 8 standards with minimal configuration.

Task 4: Format Code Using autopep8
Install autopep8:

pip install autopep8
Apply aggressive formatting:

autopep8 --in-place --aggressive --aggressive example.py
Comparison
black enforces a strict and consistent style.

autopep8 focuses on fixing PEP 8 violations and allows more flexibility.

Conclusion
In this lab, you learned how to enforce Python coding standards using PEP 8. You practiced identifying style violations with flake8 and correcting them using black and autopep8. These tools help maintain clean, readable, and professional Python code and are essential for modern development workflows.
