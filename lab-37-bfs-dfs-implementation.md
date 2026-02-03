# Lab 37: BFS/DFS Implementation (Data Structures)

## Objectives
- Understand the fundamental concepts of **Breadth-First Search (BFS)** and **Depth-First Search (DFS)**.
- Implement BFS and DFS algorithms using Python.
- Analyze traversal order differences and real-world use cases of BFS vs DFS.

## Prerequisites
- Basic understanding of graph theory and data structures
- Familiarity with Python (functions, loops, lists, dictionaries)

## Introduction
In this lab, we explore two essential graph traversal algorithms: **Breadth-First Search (BFS)** and **Depth-First Search (DFS)**. These algorithms are widely used in computer science for tasks such as shortest path finding, cycle detection, and exploring connected components in graphs.

---

## Task 1: Graph Representation

### Objective
Represent a graph using an adjacency list in Python.

### Graph Using a Dictionary
```python
graph = {
    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []
}
Key Concept – Adjacency List:
Each node stores a list of its neighboring nodes. This method is memory-efficient and commonly used for graph representations.

Task 2: Breadth-First Search (BFS)
Objective
Traverse the graph level by level using a queue.

BFS Implementation
from collections import deque

def bfs(start_node, graph):
    visited = set()
    queue = deque([start_node])

    while queue:
        node = queue.popleft()
        if node not in visited:
            print(node, end=' ')
            visited.add(node)
            queue.extend([n for n in graph[node] if n not in visited])
Key Concept – Queue:
BFS uses a queue to explore nodes in the order they are discovered.

Task 3: Depth-First Search (DFS)
Objective
Traverse the graph by exploring as deep as possible before backtracking.

DFS Implementation
def dfs(node, graph, visited=None):
    if visited is None:
        visited = set()

    if node not in visited:
        print(node, end=' ')
        visited.add(node)
        for neighbor in graph[node]:
            dfs(neighbor, graph, visited)
Key Concept – Recursion:
DFS commonly uses recursion to explore each branch completely.

Task 4: BFS vs DFS Comparison
Traversal Order
BFS: Explores nodes level by level.

DFS: Explores deep into one branch before backtracking.

Use Cases
BFS: Shortest path in unweighted graphs, level-order traversal

DFS: Cycle detection, backtracking problems, exhaustive searches

Examples
BFS: Finding the shortest route in a maze

DFS: Puzzle solving (e.g., Sudoku, maze solving)

Conclusion
In this lab, we implemented BFS and DFS using Python and explored how graph traversal works using adjacency lists. Understanding when to use BFS versus DFS is crucial for solving different types of graph-related problems efficiently. Practicing these algorithms on larger and more complex graphs will further strengthen your problem-solving skills.
