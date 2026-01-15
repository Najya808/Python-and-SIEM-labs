Lab 26: Decorators: Basic Usage
What I Learned
In this lab, I learned the basics of Python decorators. Decorators allow functions to be wrapped to extend or modify their behavior without changing their code. I practiced creating a simple logging decorator and applying it to a function.

  Lab Objectives
- Understand the concept of Python decorators
- Implement a basic decorator to enhance function behavior
- Apply decorators using the `@` syntax
- Learn practical uses such as logging and caching

  Lab Tasks Performed

 Task 1: Introduction to Python Decorators
- Decorators are functions that wrap other functions to add functionality.
- They help manage cross-cutting concerns like logging or caching.

---

 Task 2: Writing a Basic Decorator

```python
def log_decorator(func):
    def wrapper(*args, **kwargs):
        print("Start")
        result = func(*args, **kwargs)
        print("End")
        return result
    return wrapper
Explanation:

log_decorator takes a function func and returns wrapper.

wrapper prints "Start", executes func, prints "End", and returns the result.

*args and **kwargs allow the decorator to handle any number of arguments.

Task 3: Applying the Decorator
python
Copy code
@log_decorator
def say_hello(name):
    print(f"Hello, {name}!")

say_hello("Alice")
Output:

powershell
Copy code
Start
Hello, Alice!
End
Explanation:

The @log_decorator syntax applies the decorator to say_hello.

The function is wrapped, so the decorator’s functionality runs before and after the original function.

Task 4: Benefits of Using Decorators
Logging: Track function calls without modifying function code.

Caching: Store results of expensive operations for repeated use.

Modularity: Reusable functionality applied consistently across multiple functions.

 Key Concepts
Decorator: A function that wraps another function to modify its behavior.

Wrapper Function: Inner function that executes additional code before/after the original function.

@ Syntax: Shorthand to apply a decorator to a function.

 Summary
Python decorators are a powerful tool to add functionality cleanly and modularly. This lab introduced logging decorators, showing how to enhance functions without changing their internal logic. Mastering decorators allows for cleaner, reusable code across projects.
