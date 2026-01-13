Lab 10: Basic Functions
 What I Learned

In this lab, I learned how to create and use functions in Python. I practiced defining functions with parameters, calling them with arguments, using default values, and employing keyword arguments. Functions help make code modular, reusable, and more readable, which is essential for building larger programs efficiently.

🎯 Lab Objectives

Understand the concept of functions in programming

Learn to define and call functions with or without parameters

Explore default parameters and keyword arguments

Demonstrate practical usage by creating reusable code blocks

🧪 Lab Tasks Performed
🔹 Task 1: Define a Function greet(name)

Objective: Create a function that greets a user by name.

def greet(name):
    return f"Hello, {name}!"


🔍 Explanation

def keyword is used to define a function

name is a parameter that the function receives

return sends back a formatted greeting string

🔹 Task 2: Call the Function and Print Results

Objective: Execute the function with different arguments.

print(greet("Alice"))
print(greet("Bob"))
print(greet("Charlie"))


🔍 Explanation

Function calls pass a specific argument to the function

Output displays the personalized greeting for each name

Example Output:

Hello, Alice!
Hello, Bob!
Hello, Charlie!

🔹 Task 3: Use Default Parameters

Objective: Allow the function to provide a default greeting if no name is supplied.

def greet(name="Guest"):
    return f"Hello, {name}!"

print(greet())


🔍 Explanation

name="Guest" sets a default value for the parameter

If no argument is provided, the function uses "Guest"

Expected Output:

Hello, Guest!

🔹 Task 4: Utilize Keyword Arguments

Objective: Call the function using a keyword argument.

print(greet(name="Diana"))


🔍 Explanation

Keyword arguments allow passing values using parameter=value

Order of arguments is flexible

Expected Output:

Hello, Diana!

🧩 Key Concepts

Function: Reusable block of code performing a single task

Parameters: Inputs the function can accept

Return Statement: Sends output back to the caller

Default Parameters: Allow functions to work even if arguments are not provided

Keyword Arguments: Improve clarity and flexibility in function calls

✅ Summary

In this lab, I successfully:

Created functions to encapsulate reusable code

Called functions with positional and keyword arguments

Used default parameters to make functions flexible

Improved understanding of code modularity and readability

Functions are a foundational programming concept, and mastering them prepares me for more advanced topics like recursion, higher-order functions, and modular program design.
