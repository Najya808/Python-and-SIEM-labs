What I Learned

In this lab, I learned how to read and process CSV files in Python using the built-in csv module. I practiced opening CSV files, iterating over rows, handling headers, and storing data in a structured format (lists of dictionaries). This is essential for data analysis and real-world data processing tasks.

Lab Objectives

Understand how to import and use the csv module in Python.

Learn to open a CSV file and read its contents.

Iterate over rows using csv.reader().

Extract and print each row from a CSV file.

Store CSV data in a list of dictionaries.

Handle CSV files with and without headers.

🧪 Lab Tasks Performed
🔹 Task 1: Import the CSV Module
import csv

🔹 Task 2: Open and Read a CSV File
file_path = 'sample.csv'  # Path to your CSV file

with open(file_path, mode='r') as file:
    csv_reader = csv.reader(file)
    header = next(csv_reader)  # Skip header
    for row in csv_reader:
        print(row)


Explanation:

csv.reader() reads each row as a list of strings.

next(csv_reader) skips the header row.

🔹 Task 3: Handling CSV Without Headers
with open(file_path, mode='r') as file:
    csv_reader = csv.reader(file)
    for row in csv_reader:
        print(row)

🔹 Task 4: Store CSV Data in a List of Dictionaries
data_list = []

with open(file_path, mode='r') as file:
    csv_reader = csv.DictReader(file)  # Header row used as keys
    for row in csv_reader:
        data_list.append(row)

for item in data_list:
    print(item)


Explanation:

csv.DictReader() reads rows as dictionaries using the header row as keys.

Each row is appended to a list for structured data handling.

 Key Concepts

csv.reader(): Reads CSV rows as lists.

csv.DictReader(): Reads CSV rows as dictionaries using headers.

Header handling: Skip header with next() or use DictReader.

Data storage: Store CSV rows in a list for further processing.

 Summary

In this lab, I successfully:

Read CSV files with and without headers.

Converted CSV rows into Python lists and dictionaries.

Learned how to organize CSV data for practical use in programs.

CSV handling is crucial for real-world applications like data analysis, configuration files, and API data processing.
