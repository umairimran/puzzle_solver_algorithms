
# Project Title

A brief description of what this project does and who it's for

Here’s the README with emojis added and converted into proper Markdown format:

markdown
Copy
Edit
# Puzzle Solver: 8-Puzzle Problem Solver 🧩

This repository contains a Python implementation of various search algorithms (BFS, DFS, UCS, IDS) to solve the 8-puzzle problem. The goal of the 8-puzzle problem is to arrange the tiles of a 3x3 grid in a specific goal state starting from an initial configuration using valid moves.

## Algorithms Implemented 🚀:
- **Breadth-First Search (BFS)**
- **Depth-First Search (DFS)**
- **Uniform Cost Search (UCS)**
- **Iterative Deepening Search (IDS)**

These algorithms are used to search through the possible states of the 8-puzzle and find a solution, if one exists, by applying valid tile movements.

## Problem Definition 🧩:
The 8-puzzle problem consists of a 3x3 grid with 8 numbered tiles (1 to 8) and an empty space (represented as 0). The goal is to move the tiles around the grid, using the empty space, to match a given goal state from an initial configuration.

### Example:
- **Initial State:**
1 2 0
3 4 5
6 7 8

markdown
Copy
Edit

- **Goal State:**
1 2 3
4 5 6
7 8 0

markdown
Copy
Edit

### Valid Moves:
Tiles can be moved into the empty space, either left, right, up, or down, provided the move is within the grid boundaries.

## Features ✨:
- **BFS**: Explores all states level by level, ensuring the shortest path to the goal is found.
- **DFS**: Explores deeper paths first, potentially going down longer paths before backtracking.
- **UCS**: Finds the least-cost path, considering the number of moves required.
- **IDS**: Performs DFS with increasing depth limits, effectively combining the benefits of BFS and DFS.

## Installation ⚙️:
1. Clone the repository to your local machine:
 ```bash
 git clone https://github.com/yourusername/puzzle-solver.git
Install the required dependencies (if any):
bash
Copy
Edit
pip install -r requirements.txt
Usage 💻:
To use the puzzle_solver class, simply instantiate it with the initial and goal states, and then call one of the search methods (e.g., bfs(), dfs(), ucs(), or ids()).

Example:
python
Copy
Edit
initial_state = "120345678"
goal_state = "012345678"
puzzle = puzzle_solver(initial_state, goal_state)

# Run BFS
puzzle.bfs()

# Run DFS
puzzle.dfs()

# Run UCS
puzzle.ucs()

# Run IDS with a depth limit of 50
puzzle.ids(50)
Results 📊:
Each algorithm will output:

The steps it took to reach the goal.
The number of nodes visited during the search.
The time taken to find the solution.
The memory consumed during the search.
Methods 🔧:
bfs(): Implements the Breadth-First Search algorithm.
dfs(): Implements the Depth-First Search algorithm.
ucs(): Implements the Uniform Cost Search algorithm.
ids(): Implements the Iterative Deepening Search algorithm.
get_path(): Returns the path from the initial state to the goal state.
print_matrix(): Prints the current state in a 3x3 grid format.
print_results(): Prints the search results, including the number of nodes visited and the time taken.
Performance Metrics 📈:
Memory Consumed: The maximum memory used during the search.
Time Taken: The total time taken by the algorithm to find the solution.
Nodes Visited: The number of nodes explored during the search process.
Contribution 🤝:
Feel free to fork and submit pull requests. For major changes or features, please open an issue first to discuss it.

License 📜:
This project is licensed under the MIT License - see the LICENSE file for details.

