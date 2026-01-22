Lab 28: Multithreading Basics

 What I Learned
In this lab, I learned the fundamentals of multithreading in Python using the built-in `threading` module. I explored how to create and manage threads, how threads share memory, and why concurrency issues such as race conditions can occur if shared resources are not handled carefully.

 Objectives
- Understand the basics of multithreading in Python
- Learn how to create, start, and join threads
- Recognize the shared memory model used by threads
- Identify potential concurrency issues like race conditions

 Prerequisites
- Basic knowledge of Python programming
- Python installed on the system
- A code editor or IDE (VS Code, PyCharm, etc.)

---

 Lab Tasks Performed

 Task 1: Import the Threading Module

```python
import threading
Explanation:
The threading module provides tools for creating and managing threads in Python.

Task 2: Define a Function for Thread Execution
python
Copy code
def print_numbers(thread_name, start, end):
    """Prints numbers from start to end."""
    for number in range(start, end):
        print(f"{thread_name}: {number}")
Explanation:

thread_name helps identify which thread is running

start and end define the range of numbers

Each thread executes the same function with different arguments

Task 3: Create Threads
python
Copy code
thread1 = threading.Thread(target=print_numbers, args=("Thread-1", 0, 5))
thread2 = threading.Thread(target=print_numbers, args=("Thread-2", 5, 10))
Key Concepts:

Threads are lightweight subprocesses

Each thread runs concurrently

The target parameter specifies the function to execute

Task 4: Start and Join Threads
python
Copy code
thread1.start()
thread2.start()

thread1.join()
thread2.join()
Explanation:

start() begins thread execution

join() ensures the main program waits for threads to finish

Prevents premature termination of the program

Task 5: Shared Memory & Concurrency Issues
Shared Memory:

All threads operate in the same memory space

Threads can access and modify shared variables

Concurrency Issues:

Race conditions occur when multiple threads modify shared data simultaneously

Bugs caused by race conditions are difficult to detect and reproduce

Example Scenario (Race Condition):

Two threads update a bank account balance at the same time

Both read the same initial balance

Final balance becomes incorrect due to lack of synchronization

 Summary
This lab introduced multithreading in Python and demonstrated how to create, run, and synchronize threads. I learned that while multithreading improves performance through concurrency, it also introduces risks due to shared memory access. Proper synchronization is essential to avoid race conditions and ensure correct program behavior.
