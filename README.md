# London-Underground-Route-Optimisation
Optimising travel routes in the London Underground using BFS, DFS, UCS, and heuristic-based search. Efficiently finds optimal paths, compares memory usage, and analyses algorithm performance clearly.

Agenda-Based Search and Genetic Algorithms for Pathfinding
==========================================================
Author: Aditya Iyer

Project Overview
----------------
This project explores graph-search algorithms and heuristic methods for solving search problems on the London Underground network. Specifically, it implements and compares:

- Breadth-First Search (BFS)
- Depth-First Search (DFS)
- Uniform-Cost Search (UCS)
- Heuristic-Based Search
- Genetic Algorithms for optimization tasks

The project provides insights into algorithm performance, memory utilization, and optimality for practical transit route planning scenarios.

Project Structure
-----------------
.
├── agenda_based_search.py (main code implementation)
├── README.txt
└── requirements.txt

Algorithms Implemented
----------------------

1. **Breadth-First Search (BFS)**:
   - Finds the shortest path between two stations in terms of hops.
   - Explores nodes level-by-level.

2. **Depth-First Search (DFS)**
   - Used primarily for path exploration.
   - Does not guarantee the shortest or optimal path.
   - Efficient memory usage.

3. **Uniform-Cost Search (UCS)**
   - Explores paths in order of increasing path cost.
   - Uses a priority queue.
   - Guarantees optimal solutions in cost-based scenarios.

4. **Heuristic Search**
   - A modified BFS using a heuristic based on the difference in zones.
   - Guides search efficiently, reducing explored nodes significantly.

5. **Genetic Algorithm**
   - Optimizes solution search through evolution-inspired processes.
   - Implements selection (top 20%), crossover, and mutation.
   - Hyperparameter tuning performed (mutation rates tested: 0.1, 0.2).

Datasets and Testing
--------------------
The algorithms were tested using realistic London Underground station connections and costs. Pathfinding examples evaluated include routes such as:

- Tottenham Court Road to Stratford
- Baker Street to Wembley Park
- Canada Water to Stratford
- Ealing Broadway to South Kensington

Key Observations
-----------------
- **BFS**: Quickly identifies shortest paths but uses moderate memory.
- **DFS**: Efficient exploration, lowest memory, but not optimal.
- **UCS**: Guarantees cost-optimal paths, but highest memory consumption.
- **Heuristic BFS**: More guided search, fewer expansions, balanced optimality and resource utilization.
- **Genetic Algorithm**: Efficiently converges to optimized solutions with proper hyperparameter tuning.

Instructions to Run Code
------------------------
- Ensure Python is installed on your system (recommended Python 3.8 or higher).

Install Dependencies:


Dependencies
------------
- pandas
- numpy
- Python Standard Library (`heapq`, `hashlib`, `math`, `string`)

Recommended Python version: Python 3.10+

Usage
-----
- Each algorithm (BFS, DFS, UCS, Heuristic Search, Genetic Algorithm) can be run independently.
- Clearly modify parameters (stations, mutation rates, etc.) within each function or notebook as desired.

Example (Running BFS):

path, cost, nodes_expanded = bfs(graph, 'Tottenham Court Road', 'Stratford') print(f"Shortest Path: {path}") print(f"Average Time: {total_cost}") print(f"Nodes Expanded: {nodes_expanded}")


Key Observations
----------------
- There’s no universally superior search algorithm; optimality, efficiency, and memory use depend on the problem specifics.
- UCS provided optimal paths considering varying costs but required significant memory.
- BFS is ideal for simple shortest-path problems, whereas DFS excels in low-memory environments with deep search spaces.
- Genetic Algorithms benefit significantly from increased mutation rates (0.2) for faster and consistent convergence.

Future Directions
-----------------
- Apply heuristic and genetic optimization to larger datasets or real-world transit networks.
- Extend genetic algorithm with adaptive mutation rates.
- Investigate multi-objective optimization for transit scenarios, considering time, transfers, and passenger preferences.

Author
------
Aditya Iyer  
- GitHub: https://github.com/Adityaiyer3004  
- LinkedIn: https://linkedin.com/in/aditya-iyer  
- Email: adityaiyer30@gmail.com

License
-------
MIT License © Aditya Iyer


