# A-search-algorithm
# A* Pathfinding Algorithm in Python

This project implements the A* (A-Star) pathfinding algorithm in Python. It allows users to input a custom graph via the command line and find the shortest path between two nodes, optionally using heuristic values.

## ✨ Features

- Supports both Dijkstra’s algorithm (by setting all heuristics to 0) and A* algorithm.
- Allows user input for:
  - Nodes and edges in the graph
  - Start and goal nodes
  - Optional heuristic values
- Reconstructs and prints the shortest path found


## 🚀 How to Run

1. Clone this repository or copy the script to your local machine.
2. Run the script using Python:

```bash
python astar.py
Follow the prompts to:

Enter the number of nodes and edges

Define each edge with its weight

Choose whether to use heuristic values

Provide start and goal nodes

Example Interaction
mathematica
Copy
Edit
Enter the number of nodes: 3
Enter node name 1: A
Enter node name 2: B
Enter node name 3: C
Enter the number of edges: 3
Enter edge 1 (start_node end_node weight): A B 2
Enter edge 2 (start_node end_node weight): B C 3
Enter edge 3 (start_node end_node weight): A C 10
Enter the start node: A
Enter the goal node: C
Do you want to provide heuristic values for each node (yes/no)? yes
Enter heuristic value for node A: 5
Enter heuristic value for node B: 2
Enter heuristic value for node C: 0
Shortest path found: A -> B -> C
📖 How It Works
The algorithm uses a priority queue (heapq) to always explore the node with the lowest estimated total cost (f_cost = g_cost + h_cost).

You can provide your own heuristics for A*, or skip them to use Dijkstra's algorithm.

The path is reconstructed from the goal node back to the start using parent pointers.


A* is a widely used graph traversal and pathfinding algorithm.


