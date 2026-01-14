 Lab 24: Basic Regular Expressions

 What I Learned
In this lab, I learned the fundamentals of regular expressions (regex) in Python using the built-in `re` module. I practiced finding patterns, replacing text, and using groups to extract structured data from strings.

 Lab Objectives
- Understand basic concepts of regular expressions (regex)
- Learn how to use the `re` module in Python
- Find, match, and replace patterns in strings
- Use special characters and groups in regex

 Lab Tasks Performed

 Task 1: Importing the `re` Module
Regular expressions in Python are handled using the `re` module.

```python
import re
Task 2: Compiling a Regular Expression Pattern
Created a regex pattern to match digits

Used \d+ to match one or more digits

python
Copy code
pattern = re.compile(r"\d+")
Task 3: Finding All Matches in a String
Created a test string

Used findall() to extract all numeric values

python
Copy code
test_string = "The rainfall 2021 was greater than 2019 and 2020 combined."
matches = pattern.findall(test_string)
print("Matches found:", matches)
Task 4: Replacing Matches in a String
Used re.sub() to replace all digits with a placeholder

python
Copy code
replaced_string = pattern.sub("XXXX", test_string)
print("Replaced String:", replaced_string)
Task 5: Using Groups and Special Characters
Using Groups
Used parentheses () to capture parts of a pattern

Matched dates in YYYY-MM-DD format

python
Copy code
date_pattern = re.compile(r"(\d{4})-(\d{2})-(\d{2})")
date_string = "Date of birth: 1990-08-15 and starting date 2020-01-01."
date_matches = date_pattern.findall(date_string)
print("Date Matches:", date_matches)
Using Named Groups
Used named groups for better readability

python
Copy code
named_date_pattern = re.compile(
    r"(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2})"
)

named_date_matches = named_date_pattern.finditer(date_string)
for match in named_date_matches:
    print(
        "Year:", match.group("year"),
        "Month:", match.group("month"),
        "Day:", match.group("day")
    )
Key Concepts
Regular Expressions (Regex): Patterns used for matching text

re.compile(): Compiles a regex pattern for reuse

findall(): Finds all matches in a string

sub(): Replaces matched patterns

Groups: Capture specific parts of a pattern

Named Groups: Improve clarity and readability

 Summary
This lab introduced me to the power of regular expressions in Python. I learned how to search, replace, and extract structured information from text using regex patterns and groups. These skills are essential for text processing, data validation, log analysis, and working with real-world datasets.
