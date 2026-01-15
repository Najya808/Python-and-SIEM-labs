 Lab 27: Context Managers (with statement)

 What I Learned
In this lab, I learned how context managers in Python simplify resource management. They ensure that resources like files, sockets, or database connections are properly acquired and released, even if exceptions occur. I also practiced creating a custom context manager using `__enter__` and `__exit__` methods.

 Lab Objectives
- Understand context managers and the `with` statement
- Create a custom context manager class with `__enter__` and `__exit__`
- Automatically manage resources and cleanup
- Ensure safe execution even in the presence of exceptions

 Lab Tasks Performed

 Task 1: Introduction to Context Managers
- Context managers manage the setup and teardown of resources.
- The `with` statement automatically calls `__enter__` at the start and `__exit__` at the end of a block.
- Key concept: Simplifies exception handling and ensures resources are released.

---

 Task 2: Creating a Custom Context Manager Class

```python
class MyContext:
    def __enter__(self):
        print("Entering the context and allocating resources.")
        return self
    
    def __exit__(self, exc_type, exc_value, traceback):
        print("Exiting the context and cleaning up resources.")

 Using the custom context manager
with MyContext() as context:
    print("Running within the context block.")
Output:

sql
Copy code
Entering the context and allocating resources.
Running within the context block.
Exiting the context and cleaning up resources.
Explanation:

__enter__: Sets up the resource and returns it for use in the with block.

__exit__: Automatically called at block exit, cleaning up resources safely, even if an exception occurs.

Task 3: File Management Example Using Context Managers
python
Copy code
class FileManager:
    def __init__(self, filename, mode):
        self.filename = filename
        self.mode = mode
    
    def __enter__(self):
        self.file = open(self.filename, self.mode)
        return self.file
    
    def __exit__(self, exc_type, exc_value, traceback):
        self.file.close()

# Using FileManager context manager
with FileManager('sample.txt', 'w') as f:
    f.write("Hello, World!")
Explanation:

The FileManager context manager ensures the file is automatically closed after writing.

This prevents resource leaks and simplifies file operations.

Task 4: Key Takeaways
Context managers are essential for safe resource management.

__enter__ sets up resources; __exit__ guarantees cleanup.

Works for files, network connections, locks, or any resource that requires cleanup.

Makes code cleaner, safer, and less error-prone.

 Summary
Context managers in Python provide a robust way to handle resources automatically. By creating custom classes with __enter__ and __exit__, I can ensure proper setup and teardown. The with statement simplifies coding patterns, reduces boilerplate, and ensures consistent resource management.
