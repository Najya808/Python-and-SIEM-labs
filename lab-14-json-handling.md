What I Learned

In this lab, I learned how to work with JSON data in Python. I practiced converting Python dictionaries to JSON strings, storing JSON data in files, and reading it back into Python objects. This lab taught me the importance of JSON for configuration, data storage, and data interchange, particularly in modern web applications and APIs.

🎯 Lab Objectives

Understand how to create a Python dictionary and convert it to JSON

Learn how to store JSON data in a file and read it back

Comprehend the use of JSON for configuration and data exchange

🧪 Lab Tasks Performed

🔹 Task 1: Create and Convert a Python Dictionary to JSON

Step 1: Create a Python Dictionary

# Create a Python dictionary
employee_data = {
    "name": "John Doe",
    "age": 30,
    "department": "Engineering",
    "skills": ["Python", "Django", "Machine Learning"]
}


Explanation:

Python dictionaries store key-value pairs.

Dictionaries are versatile for representing structured data.

Step 2: Convert the Dictionary to a JSON String

import json

# Convert the dictionary to a JSON string
employee_data_json = json.dumps(employee_data, indent=4)
print(employee_data_json)


Explanation:

json.dumps() converts a Python object to a JSON-formatted string.

indent=4 is used for readability.

🔹 Task 2: Store JSON Data in a File

Step 1: Write JSON to a File

# Write JSON data to a file
with open("employee_data.json", "w") as json_file:
    json_file.write(employee_data_json)


Explanation:

Uses Python’s file handling (open() in write mode).

Context managers (with) ensure the file is closed properly.

Step 2: Read JSON Data from the File

# Read JSON data from the file
with open("employee_data.json", "r") as json_file:
    data = json.load(json_file)
    print(data)


Explanation:

json.load() parses a JSON file and converts it back into a Python dictionary.

Useful for reading configuration or structured data back into the program.

🔹 Task 3: Summarize JSON Usage

Discussion:

JSON for Configuration: Lightweight and human-readable, ideal for storing application settings.

Data Interchange: Language-independent format used for APIs and web services.

Case Study Example: Fetching weather data from an API returns JSON, which can be processed in Python for GUI or reporting.

🧩 Key Concepts

json.dumps(): Converts Python object to JSON string

json.load(): Converts JSON data back into a Python object

Context managers (with): Ensures safe file handling

Data interchange & storage: JSON is widely used in modern software applications

 Summary

Converted Python dictionaries to JSON and back.

Stored JSON data in files and read it efficiently.

Understood the relevance of JSON in real-world applications like APIs and configurations.

Gained practical skills for handling structured data in Python.
