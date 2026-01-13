What I Learned

In this lab, I learned how to organize Python code using modules and packages. I practiced creating a custom module with functions, importing it in another script, and structuring packages for better code organization. This lab helped me understand code reusability and maintainability, which is essential for larger projects.

🎯 Lab Objectives

Understand Python modules and how to use them

Learn to import and utilize functions from modules

Recognize the structure and purpose of packages

Practice creating your own modules and packages

🧪 Lab Tasks Performed

🔹 Task 1: Creating and Using a Python Module

Step 1: Create a Module

# Filename: mymodule.py

def add(a, b):
    """Returns the sum of two numbers."""
    return a + b


Step 2: Use the Module in a Script

# Filename: main.py

import mymodule

# Call the add function from mymodule
result = mymodule.add(5, 3)
print(f"The sum of 5 and 3 is {result}")


Step 3: Run the Script

python main.py


Expected Output:

The sum of 5 and 3 is 8


🔍 Explanation:

A module is a Python file (.py) containing functions, classes, or variables.

Using import mymodule allows us to access functions defined in mymodule.py.

🔹 Task 2: Creating and Using a Python Package

Step 1: Create Package Structure

mypackage/
│
├── __init__.py
└── mymodule.py


Step 2: Import from the Package

# Filename: main.py

from mypackage import mymodule

result = mymodule.add(5, 3)
print(f"The sum of 5 and 3 is {result}")


Step 3: Run the Script

python main.py


Expected Output:

The sum of 5 and 3 is 8


🔍 Explanation:

Package: A directory with __init__.py containing modules.

Modules can be imported using from package import module.

Packages help organize code and improve maintainability in large projects.

🧩 Key Concepts

Module: A single Python file containing code (functions, classes, variables).

Package: A directory of modules with __init__.py to treat it as a package.

Code Reusability: Modules and packages allow us to use code in multiple scripts without duplication.

Summary

Created a Python module and used it in another script.

Created a package with an __init__.py file and imported modules from it.

Learned how modules and packages improve code organization, reusability, and maintainability.
