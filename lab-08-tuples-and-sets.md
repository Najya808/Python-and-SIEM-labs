Lab 8: Tuples & Sets
🧠 What I Learned

In this lab, I explored two important Python data structures: tuples and sets. I learned that tuples are immutable, meaning their values cannot be changed once created, making them suitable for fixed data. I also learned that sets are unordered collections of unique elements, which makes them ideal for removing duplicates and performing fast membership checks.

This lab strengthened my understanding of when and why to use tuples versus sets in real-world Python applications.

🎯 Lab Objectives

Understand the properties and usage of tuples

Understand the properties and usage of sets

Learn how to manipulate tuples and sets using practical examples

🧪 Lab Tasks Performed
🔹 Task 1: Working with Tuples
🔸 Subtask 1.1: Create a Tuple of Coordinates
Objective

Create a tuple to store fixed coordinate values.

Code
# Creating a tuple representing coordinates (x, y, z)
coordinates = (10, 20, 30)
print("Coordinates Tuple:", coordinates)

🔍 Explanation

Tuples are created using parentheses ()

The tuple stores multiple related values together

Tuples can hold different data types

Commonly used for fixed data such as coordinates

🔸 Subtask 1.2: Confirm Tuple Immutability
Objective

Demonstrate that tuples cannot be modified after creation.

Code
# Attempt to change the x-coordinate
try:
    coordinates[0] = 100
except TypeError as e:
    print("Error:", e)

🔍 Explanation

Tuples are immutable

Attempting to modify a tuple element raises a TypeError

Immutability helps protect data from accidental modification

🔹 Task 2: Working with Sets
🔸 Subtask 2.1: Create a Set of Numbers
Objective

Create a set to store unique numbers.

Code
# Create a set of numbers
number_set = {1, 2, 3, 4, 5}
print("Initial Set:", number_set)

🔍 Explanation

Sets are defined using curly braces {}

Elements in a set are unordered

Duplicate values are automatically removed

🔸 Subtask 2.2: Add a Duplicate and Observe Behavior
Objective

Verify that sets do not allow duplicate values.

Code
# Attempt to add a duplicate number to the set
number_set.add(3)
print("Set after adding duplicate:", number_set)

🔍 Explanation

Adding a duplicate value has no effect

Sets always maintain unique elements only

This makes sets ideal for deduplication tasks

🧩 Key Concepts

Tuple: An ordered, immutable collection of elements

Immutability: Data cannot be changed after creation

Set: An unordered collection of unique elements

Deduplication: Removing duplicate values from data

Membership Testing: Quickly checking if an element exists

 Summary

In this lab, I successfully:

Created and used tuples for fixed data storage

Demonstrated tuple immutability through error handling

Created sets and observed automatic duplicate removal

Understood real-world use cases for tuples and sets

These data structures are essential for writing efficient, clean, and reliable Python programs.
