What I Learned

In this lab, I learned how to handle file input/output (I/O) in Python, including reading from and writing to files. I practiced using context managers with the with statement to ensure files are safely opened and closed. This lab helped me understand how Python efficiently manages file resources and how to perform basic file operations safely and reliably.

🎯 Lab Objectives

Understand the basic concepts of File I/O in Python

Learn how to read from and write to files

Utilize context managers to manage files efficiently

🧪 Lab Tasks Performed

🔹 Task 1: Writing to a File

Objective: Write data to a file named output.txt.

# Filename: write_file.py

# Open the file output.txt in write mode
with open('output.txt', 'w') as f:
    # Write multiple lines to the file
    f.write("Hello, World!\n")
    f.write("This is a file I/O example.\n")
    f.write("Python makes File I/O easy!\n")


Explanation:

'w' mode opens the file for writing and overwrites existing data.

The with statement is a context manager that automatically closes the file after the block finishes.

🔹 Task 2: Reading from a File

Objective: Read the contents of output.txt line by line.

# Filename: read_file.py

# Open the file output.txt in read mode
with open('output.txt', 'r') as f:
    # Read each line in the file
    for line in f:
        # Print the line to the console
        print(line.strip())


Explanation:

'r' mode opens the file for reading.

line.strip() removes extra whitespace and newlines from each line.

The context manager ensures the file is closed properly, even if an error occurs.

🔹 Task 3: Understanding Context Managers

Explanation:

Context managers automate resource management, like opening and closing files.

Using with reduces the risk of file corruption and ensures proper cleanup.

They simplify exception handling and improve code readability and reliability.

🧩 Key Concepts

File I/O: Reading from and writing to files using Python.

Write Mode ('w'): Overwrites the file or creates a new file if it doesn't exist.

Read Mode ('r'): Reads file contents line by line.

Context Manager (with): Ensures safe and automatic closing of files.

Summary

Wrote multiple lines to a file using Python.

Read file contents and processed them line by line.

Learned the importance of context managers in file handling.

Gained foundational knowledge for handling data files safely in Python projects.
