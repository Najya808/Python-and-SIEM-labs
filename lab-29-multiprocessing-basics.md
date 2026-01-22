Lab 29: Multiprocessing Basics

 What I Learned
In this lab, I learned how Python handles multiprocessing for CPU-bound tasks using the `multiprocessing` module. I explored how to create and run multiple processes in parallel, understood how processes differ from threads, and learned why multiprocessing is better suited for CPU-intensive workloads due to separate memory spaces.

---

 Objectives
- Understand the basics of multiprocessing in Python
- Learn how to create and manage multiple processes
- Differentiate between multiprocessing and multithreading
- Recognize how multiprocessing improves performance for CPU-bound tasks

---

 Prerequisites
- Basic knowledge of Python programming
- Familiarity with threading concepts
- Python installed on the system

---

 Lab Tasks Performed

 Task 1: Introduction to Multiprocessing

Multiprocessing allows Python programs to execute tasks in parallel using **separate processes**. Unlike threads, each process has its own memory space, which helps avoid data corruption and makes multiprocessing ideal for CPU-bound tasks.

---

 Task 2: Import the Multiprocessing Module

```python
import multiprocessing
Explanation:
The multiprocessing module provides tools for creating processes that run independently and concurrently.

Task 3: Define a CPU-Bound Function
python
Copy code
def sum_large_list(num_list):
    total = sum(num_list)
    print(f"Sum of the list is: {total}")
Explanation:
This function performs a CPU-intensive operation by summing a large list of numbers.

Task 4: Create and Start Multiple Processes
python
Copy code
numbers = list(range(1000000))

if __name__ == '__main__':
    process1 = multiprocessing.Process(target=sum_large_list, args=(numbers,))
    process2 = multiprocessing.Process(target=sum_large_list, args=(numbers,))

    process1.start()
    process2.start()

    process1.join()
    process2.join()
Key Concepts:

Each Process runs independently

start() begins process execution

join() ensures the main program waits for processes to complete

The if __name__ == '__main__' guard is required to prevent infinite process spawning

Task 5: Observing Parallel Execution
Both processes run simultaneously

Each process executes its own instance of sum_large_list

Output may appear in any order due to parallel execution

 Practical Case Study
Image Processing Example:
When applying CPU-heavy filters to multiple images, multiprocessing allows each image to be processed in parallel by different CPU cores, significantly reducing execution time.

 Summary
This lab demonstrated how multiprocessing enables true parallel execution in Python. I learned how to create and manage multiple processes, why multiprocessing is better for CPU-intensive tasks, and how it differs fundamentally from threading due to isolated memory spaces.
