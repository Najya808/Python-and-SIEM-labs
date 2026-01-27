lab-31-cli-argparse.md
Lab 31: CLI Applications with argparse

## Objectives
- Understand the basics of creating Command Line Interface (CLI) applications using Python.
- Learn how to use the argparse module to parse command-line arguments.
- Develop a simple CLI application that takes user input and produces output.
- Explore argparse’s automatic help and usage generation.

## Prerequisites
- Basic understanding of Python programming.
- Python installed on your system.
- Familiarity with command-line usage.

---

## Introduction
The `argparse` module helps developers build user-friendly command-line tools. It automatically parses arguments, validates input, and generates helpful usage messages, making scripts easier to use and maintain.

---

## Task 1: Verify Python Installation
Check that Python is installed:
```bash
python --version
Task 2: Create a CLI Script
Create a new Python file named greet.py.

Task 3: Import argparse
python
Copy code
import argparse
Task 4: Define and Parse Arguments
python
Copy code
import argparse

parser = argparse.ArgumentParser(
    description="A simple greeting application."
)

parser.add_argument(
    "--name",
    type=str,
    help="The name of the person to greet."
)

args = parser.parse_args()
Task 5: Use Parsed Arguments
python
Copy code
if args.name:
    print(f"Hello, {args.name}!")
else:
    print("Hello, Stranger!")
Task 6: Run the Script
Examples:

bash
Copy code
python greet.py --name Alice
Output:

Copy code
Hello, Alice!
bash
Copy code
python greet.py
Output:

Copy code
Hello, Stranger!
Task 7: View Help Text
bash
Copy code
python greet.py --help
Argparse automatically generates usage instructions and argument descriptions.

Conclusion
In this lab, you learned how to:

Create a basic CLI application in Python.

Parse command-line arguments using argparse.

Use parsed arguments to control program behavior.

Leverage argparse’s built-in help system.

These skills are essential for building professional command-line tools and automation scripts.
