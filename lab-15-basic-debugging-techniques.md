What I Learned

In this lab, I learned how to debug Python programs using print statements and the Python Debugger (pdb). I understood how debugging helps identify logical errors, track variable values, and analyze program flow. This lab improved my ability to locate bugs efficiently instead of guessing what went wrong.

🎯 Lab Objectives

Understand and apply basic debugging techniques in Python

Learn how to use print statements for tracing program execution

Gain familiarity with the Python Debugger (pdb)

Learn how to step through code and use breakpoints

🧪 Lab Tasks Performed

🔹 Task 1: Using Print Statements for Debugging

Objective:
Track variable values during execution using print statements.

Code Example:

def calculate_sum(numbers):
    total = 0
    for num in numbers:
        total += num
        print("Debug: Adding", num, "Total so far:", total)
    return total

# Test the function
numbers = [5, 10, 15]
print("Final Sum:", calculate_sum(numbers))


🔍 Explanation

Print statements display intermediate values

Helps track how variables change step-by-step

Useful for finding logic errors in loops and calculations

🔹 Task 2: Introduction to Python Debugger (pdb)

Objective:
Use pdb to pause execution and inspect code behavior.

Code Example:

def divide_numbers(a, b):
    import pdb; pdb.set_trace()
    result = a / b
    print("Result:", result)
    return result

divide_numbers(10, 0)


🔍 Explanation

pdb.set_trace() sets a breakpoint

Execution pauses, allowing inspection of variables

Useful for complex debugging scenarios

🔹 Task 3: Step Through Code Execution Using pdb

Objective:
Understand program flow and locate errors interactively.

Common pdb Commands Used:

n → Execute next line

s → Step into a function

c → Continue execution

q → Quit debugger

print(a, b) → Inspect variable values

🔍 Explanation

Helps identify exactly where errors occur

Essential for debugging runtime and logical errors

More powerful than print statements for large programs

🧩 Key Concepts

Print Debugging: Simple and quick method to trace values

pdb: Python’s built-in interactive debugger

Breakpoints: Pause execution at a specific line

Step-by-step execution: Understand program logic clearly

Summary

In this lab, I successfully:

Debugged code using print statements

Used pdb to pause and inspect execution

Learned essential debugging commands

Improved problem-solving and error-tracing skills

Debugging is a critical skill for writing reliable and maintainable Python programs.
