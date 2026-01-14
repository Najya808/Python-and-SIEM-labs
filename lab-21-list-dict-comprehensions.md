What I Learned

In this lab, I learned how to use list comprehensions and dictionary comprehensions to create data structures in Python more efficiently. I discovered how these concise constructs replace traditional loops, improve code readability, and can even offer better performance for certain tasks. This lab enhanced my understanding of Pythonic ways to manipulate lists and dictionaries.

 Lab Objectives

Understand the syntax and use of list comprehensions

Learn dictionary comprehensions for mapping keys to values

Improve code readability and efficiency

Compare comprehensions with traditional loop-based methods

 Prerequisites

Basic Python knowledge

Familiarity with lists, dictionaries, and loops

Understanding of basic control structures in Python

🧪 Lab Tasks Performed

🔹 Task 1: Create a List of Squares Using List Comprehension

# Using list comprehension to generate squares
squares = [x**2 for x in range(10)]
print(squares)


Explanation:

Iterates over numbers 0 to 9

Computes x**2 for each number

Adds each result to the list squares

Result:

[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]


🔹 Task 2: Build a Dictionary from a List of Strings Using Dictionary Comprehension

# List of strings
words = ["apple", "banana", "cherry", "date"]

# Dictionary comprehension to map words to their lengths
lengths = {word: len(word) for word in words}
print(lengths)


Explanation:

Iterates over each word in the list words

Maps the word to its length using len(word)

Stores key-value pairs in the dictionary lengths

Result:

{'apple': 5, 'banana': 6, 'cherry': 6, 'date': 4}


🔹 Task 3: Advantages of Using Comprehensions

Simplification and Readability:

Comprehensions replace loops with concise code

Example using a loop vs comprehension:

# Using a loop
squares_loop = []
for x in range(10):
    squares_loop.append(x**2)

# Using list comprehension
squares_comp = [x**2 for x in range(10)]


Comparison:

Comprehensions are shorter, cleaner, and reduce potential errors

Often optimized internally for better performance

Use Cases:

Data transformations, filtering, mapping values

Efficiently creating lists or dictionaries in one line

 Conclusion

List and dictionary comprehensions provide concise, readable, and maintainable code

They replace traditional loops for many use cases

Understanding comprehensions enhances Python proficiency and leads to more efficient coding practices
They replace traditional loops for many use cases

Understanding comprehensions enhances Python proficiency and leads to more efficient coding practices
