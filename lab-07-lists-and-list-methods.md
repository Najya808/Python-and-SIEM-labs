Lab 7: Lists & List Methods
 What I Learned

In this lab, I learned how to work with lists in Python, which are one of the most commonly used data structures. I practiced creating lists, modifying their contents, and using built-in list methods such as append(), remove(), and sort(). I also learned how to iterate over lists using loops to access each element.

This lab helped me understand how Python manages collections of data efficiently and how lists can be dynamically updated during program execution.

🎯 Lab Objectives

Understand the concept of lists in Python

Learn how to create and modify lists

Use common list methods to manage data

Iterate through lists using loops

🧪 Lab Tasks Performed
🔹 Task 1: Create a List of Fruits
Objective

Create a list and print its contents.

Code
fruits = ["apple", "banana", "cherry"]
print("Initial list of fruits:", fruits)

Explanation

A list is created using square brackets []

Each item in the list is a string

The print() function displays the list contents

🔹 Task 2: Append a New Fruit
Objective

Add a new element to the list using append().

Code
fruits.append("orange")
print("List after appending 'orange':", fruits)

Explanation

append() adds an element to the end of the list

Lists are mutable, meaning they can be changed after creation

🔹 Task 3: Remove a Fruit by Name
Objective

Remove an existing element from the list.

Code
fruits.remove("banana")
print("List after removing 'banana':", fruits)

Explanation

remove() deletes the specified element by value

The element must exist in the list, otherwise an error occurs

🔹 Task 4: Sort the List
Objective

Sort list elements in ascending order.

Code
fruits.sort()
print("Sorted list of fruits:", fruits)

Explanation

sort() arranges items alphabetically by default

The original list is modified in place

🔹 Task 5: Iterate Over the List
Objective

Access each element in the list using a loop.

Code
for fruit in fruits:
    print("Fruit:", fruit)

Explanation

The for loop goes through each item in the list

Each element is stored temporarily in the variable fruit

 Key Concepts

List: An ordered, mutable collection of items

append(): Adds an element to the end of a list

remove(): Removes an element by value

sort(): Orders elements in ascending order

Iteration: Accessing elements one by one using a loop

Summary

In this lab, I successfully:

Created and displayed a list

Modified the list using built-in methods

Sorted list elements alphabetically

Iterated through list items using a loop

Lists are essential for handling multiple values efficiently and are widely used in real-world Python applications such as data processing, automation, and analysis.
