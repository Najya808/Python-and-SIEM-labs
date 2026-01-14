What I Learned

In this lab, I learned how recursion works in Python and how to implement it to solve problems like calculating factorials. I practiced defining a base case and a recursive call, explored the differences between recursion and iteration, and learned about tail recursion for efficiency. This lab helped me understand when to use recursion and how it can simplify problem-solving for naturally recursive tasks.

Lab Objectives

Understand the concept of recursion in programming

Implement a recursive solution for calculating factorials

Learn differences between recursion and iteration

Explore advanced topics like tail recursion

📋 Prerequisites

Basic understanding of programming concepts

Familiarity with Python syntax and functions

Access to a Python interpreter (Python 3.x)

🧪 Lab Tasks Performed

🔹 Task 1: Introduction to Recursion

Definition: Recursion is when a function calls itself to solve smaller instances of the same problem.

Key Characteristics:

Base Case: Stops the recursion

Recursive Call: Function calls itself with modified arguments

🔹 Task 2: Implement Recursive Factorial Function

def factorial(n):
    # Base case
    if n <= 1:
        return 1
    # Recursive case
    else:
        return n * factorial(n - 1)

# Example usage
result = factorial(5)
print("The factorial of 5 is:", result)


🔍 Explanation

Base case returns 1 when n <= 1

Recursive case multiplies n by factorial of n-1

Tested with different values to verify correctness

🔹 Task 3: Recursion vs Iteration

Iterative Factorial Example:

def iterative_factorial(n):
    result = 1
    for i in range(2, n + 1):
        result *= i
    return result

# Example usage
iter_result = iterative_factorial(5)
print("The factorial of 5 using iteration is:", iter_result)


Comparison:

Recursion: Elegant and readable, naturally matches recursive problems

Iteration: More memory-efficient, avoids stack overflow

🔹 Task 4: Tail Recursion and Large Inputs

Tail Recursive Factorial Example:

def tail_recursive_factorial(n, accumulator=1):
    if n <= 1:
        return accumulator
    else:
        return tail_recursive_factorial(n - 1, n * accumulator)

# Example usage
tail_result = tail_recursive_factorial(5)
print("The factorial of 5 using tail recursion is:", tail_result)


Key Points:

Tail recursion performs the recursive call as the last operation

Useful for optimizing memory usage

Iterative solutions are safer for very large inputs to prevent stack overflow

🧩 Key Concepts Covered

Base case and recursive calls in functions

Factorial computation using recursion

Differences between recursion and iteration

Tail recursion as an optimization technique

 Conclusion

In this lab, I successfully:

Implemented a recursive function to calculate factorials

Compared recursion and iteration

Explored tail recursion for memory-efficient recursion

Recursion is a powerful tool, but it should be used thoughtfully depending on problem size and memory considerations. Mastering recursion is important for solving divide-and-conquer problems and other recursive algorithms.
