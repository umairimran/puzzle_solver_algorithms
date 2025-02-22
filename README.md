8-Puzzle Solver: A Comprehensive Search Algorithm Implementation 🧩
This repository presents a robust Python implementation of multiple search algorithms (BFS, DFS, UCS, and IDS) designed to solve the classic 8-puzzle problem. The aim of the 8-puzzle problem is to systematically rearrange the tiles of a 3x3 grid, starting from a specified initial configuration, to achieve a predefined goal state using valid tile movements.

Algorithms Implemented 🚀:
Breadth-First Search (BFS): Guarantees the shortest path solution by exploring all possible states layer by layer.
Depth-First Search (DFS): Explores deeper paths first, potentially diverging down lengthy sequences before backtracking.
Uniform Cost Search (UCS): Prioritizes finding the least-cost path, where cost is defined by the number of moves required.
Iterative Deepening Search (IDS): Combines the strengths of DFS and BFS by iteratively deepening the depth limit, providing optimal space complexity while ensuring the discovery of the shortest path.
These algorithms comprehensively search the state space of the 8-puzzle and attempt to find a solution, if one exists, by applying valid movements to the tiles.

Problem Definition 🧩:
The 8-puzzle problem involves a 3x3 grid consisting of 8 numbered tiles (ranging from 1 to 8) and one empty space, denoted as '0'. The goal is to rearrange the tiles by sliding them into the empty space until the configuration matches a given goal state.

Example:
Initial State:

Copy
1 2 0
3 4 5
6 7 8
Goal State:

Copy
1 2 3
4 5 6
7 8 0
Valid Moves:
The empty space ('0') can be moved in one of four directions: left, right, up, or down, provided the move is within the boundaries of the 3x3 grid.
Features ✨:
Breadth-First Search (BFS): Explores all potential states level by level, ensuring that the algorithm identifies the shortest path to the goal configuration in terms of moves.
Depth-First Search (DFS): Dives into deeper state spaces first, potentially exploring longer paths before backtracking to find the solution.
Uniform Cost Search (UCS): Focuses on finding the least-cost path by considering the cost associated with each transition (i.e., the number of moves).
Iterative Deepening Search (IDS): Combines the iterative nature of DFS with depth bounds, increasing the depth limit in each iteration to strike a balance between space efficiency and optimality.
Installation ⚙️:
To get started, follow these steps:

Clone the repository to your local machine:

bash
Copy
git clone https://github.com/yourusername/puzzle-solver.git
Install the required dependencies (if any) using pip:

bash
Copy
pip install -r requirements.txt
Usage 💻:
To utilize the puzzle_solver class, instantiate it by providing the initial and goal states, and then invoke one of the search methods (e.g., bfs(), dfs(), ucs(), or ids()).

Example:
python
Copy
# Define the initial and goal states as strings.
initial_state = "120345678"
goal_state = "012345678"

# Create an instance of the puzzle_solver class.
puzzle = puzzle_solver(initial_state, goal_state)

# Execute BFS
puzzle.bfs()

# Execute DFS
puzzle.dfs()

# Execute UCS
puzzle.ucs()

# Execute IDS with a specified depth limit of 50
puzzle.ids(50)
Results 📊:
Each search algorithm provides the following output:

The sequence of steps taken to reach the goal state.
The total number of nodes visited during the search.
The time consumed in finding the solution.
The memory consumed during the search process.
Methods 🔧:
bfs(): Implements the Breadth-First Search algorithm.
dfs(): Implements the Depth-First Search algorithm.
ucs(): Implements the Uniform Cost Search algorithm.
ids(): Implements the Iterative Deepening Search algorithm.
get_path(): Returns the sequence of moves (path) from the initial state to the goal state.
print_matrix(): Prints the current state of the puzzle in a user-friendly 3x3 grid format.
print_results(): Outputs the performance statistics, including the number of nodes visited and the time taken by the algorithm.
Performance Metrics 📈:
Memory Consumed: Tracks the peak memory usage during the search process.
Time Taken: The total time consumed by the algorithm to find the solution, from the initial state to the goal state.
Nodes Visited: The total number of nodes (states) explored throughout the search process.
Contribution 🤝:
We welcome contributions! Feel free to fork this repository and submit pull requests. For major changes or new features, kindly open an issue first to discuss the proposed changes.
