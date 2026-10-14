
# SLE-4: Final Viva & Architecture Decision Record (ADR)

## Course Information
- **Course:** 02AML204 – Introduction to Artificial Intelligence
- **Student Name:** Shivraj Pravin Banne
- **Division:** B
- **Date:** 12-10-2026

## Project Title
**Comparative Evaluation of BFS and DFS Using Queue and Stack for Tree Search**

## 1. Introduction
This project implements and compares two tree search algorithms: Breadth-First Search (BFS) and Depth-First Search (DFS).

The algorithms search a tree containing 15 nodes, from A to O, starting from the root node A. The project studies how their traversal methods affect the number of nodes expanded and execution time.

## 2. Objectives
- Implement BFS and DFS using Python.
- Understand the difference between queue and stack.
- Search for different goal nodes in a tree.
- Measure execution time and count expanded nodes.
- Compare the performance of both algorithms using repeated experiments.
- Document the design decisions using an Architecture Decision Record (ADR).

## 3. Technologies Used
- **Programming Language:** Python
- **Data Structures:** Queue and Stack
- **Python Module:** `collections.deque`
- **Timing:** Python `time` module
- **Profiling:** `cProfile`

## 4. Algorithms Used

### Breadth-First Search (BFS)
BFS explores the tree level by level. It uses a queue implemented with Python's `deque`. The `popleft()` operation removes the oldest node from the queue.

### Depth-First Search (DFS)
DFS explores one branch deeply before moving to another branch. It uses a Python list as a stack. The `pop()` operation removes the most recently added node.

## 5. Tree Structure
The project uses a binary tree containing 15 nodes:

- Root: A
- Second level: B, C
- Third level: D, E, F, G
- Leaf level: H, I, J, K, L, M, N, O

## 6. Experimental Method
The algorithms are tested using different goal nodes:
- B: Intended best-case goal
- M: Intended average-case goal
- O: Intended worst-case goal

Each timing run uses 5,000 repetitions, with five runs for each test case, as documented in the experiment.

Execution time and expanded nodes are used to compare the algorithms. The actual results should be taken from the final program output.

## 7. Key Observations
- BFS explores nodes level by level.
- DFS explores a branch deeply before backtracking.
- BFS uses a queue, while DFS uses a stack.
- Execution time and the number of expanded nodes are different performance measures.
- Neither algorithm is always faster for every search problem.
- Results depend on the tree structure, goal location, implementation and measurement conditions.

## 8. Advantages
- Demonstrates two important AI search algorithms.
- Provides practical understanding of queues and stacks.
- Uses repeated experiments for performance comparison.
- Makes the algorithms easier to compare through separate functions.

## 9. Limitations
- The experiment uses one fixed tree.
- Execution times are extremely small and can be affected by measurement overhead.
- Results may differ on larger or differently structured trees.

## 10. How to Run
1. Install Python 3.
2. Open the project folder in VS Code or a terminal.
3. Run the Python implementation:

   `python tree_search.py`

4. Observe the traversal, execution time and expanded-node results printed by the program.

Replace `tree_search.py` with your actual Python filename if it is different.

## 11. Conclusion
This project provides a practical comparison of BFS and DFS for tree search. It demonstrates how queue and stack operations influence traversal behaviour and how execution time and nodes expanded can be used to study algorithm performance.

The experiment shows that algorithm selection depends on the requirements and structure of the search problem.

## 12. References
- SLE-1: Tree Search Implementation
- SLE-2: Profiling and Comparison Report
- SLE-3: Tree Search Architecture Diagrams, if prepared
- Python documentation: https://docs.python.org/3/
