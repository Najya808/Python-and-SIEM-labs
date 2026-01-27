Lab: Simple Scripting for File Management

## Objectives
- Understand basic file management using Python scripts.
- Learn how to list, copy, and optionally rename files using scripting.
- Explore how scripting can offer greater flexibility compared to manual file operations.

## Prerequisites
- Basic understanding of Python programming.
- Access to a computer with Python installed.
- Familiarity with running Python scripts in a command-line interface or an IDE.

## Lab Tasks

### Task 1: Import Required Modules
We will use Python's `os` and `shutil` modules to manage files.

```python
import os
import shutil
Task 2: List Files in a Folder
Create a Python script to list all files in a directory using os.listdir().

python
Copy code
directory = 'path/to/source/folder'
files = os.listdir(directory)
print("Files in Directory:", files)
This allows you to view all files present in the specified directory.

Task 3: Copy Files to Another Folder
Use shutil.copy() to copy files to a destination directory.

python
Copy code
destination = 'path/to/destination/folder'

if not os.path.exists(destination):
    os.makedirs(destination)

for file in files:
    shutil.copy(os.path.join(directory, file), destination)
This ensures the destination folder exists before copying files.

Task 4 (Optional): Rename Files While Copying
Append _backup to each file name while copying.

python
Copy code
for file in files:
    base, extension = os.path.splitext(file)
    new_name = f"{base}_backup{extension}"
    shutil.copy(
        os.path.join(directory, file),
        os.path.join(destination, new_name)
    )
This is useful for creating backup versions of files.

Summary: Advantages of Script-Based File Management
Automation: Write once, run many times.

Scalability: Easily manage thousands of files.

Accuracy: Reduces human error.

Customization: Add logic, logging, or conditions as needed.

Conclusion
In this lab, you learned how to use Python scripting with the os and shutil modules to manage files efficiently. Automating file operations saves time, improves accuracy, and provides a foundation for more advanced scripting and system automation tasks.
