# MazeSolver

MazeSolver is a Python class that finds an optimal path through a maze, collecting coins along the way. The goal is to reach the last row while avoiding obstacles (value 1) and collecting coins (value 2).

## Usage

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/LampStack/MazeProblem.git
    cd MazeSolver
    ```

2. **Run the Example:**
    ```python
    from maze_solver import MazeSolver

    maze_input = [
        [0, 1, 1, 1, 1],
        [0, 0, 0, 2, 1],
        [1, 0, 1, 1, 1],
        [1, 0, 0, 2, 0]
    ]

    solver = MazeSolver(maze_input)
    print("Optimal Path:", solver.path)
    print("Collected Coins:", solver.coins)
    ```

3. **Expected Output:**
    ```
    Optimal Path: [[0, 0], [1, 0], [1, 1], [1, 2], [2, 2], [3, 2], [3, 3], [3, 4]]
    Collected Coins: [[1, 3], [3, 3], [3, 4]]
    ```

## Class Methods

### `MazeSolver(matrix: list) -> None`

- **Description:** Initializes the MazeSolver with a given maze matrix.
- **Parameters:**
  - `matrix` (list): A 2D list representing the maze.

### `is_valid_move(x: int, y: int) -> bool`

- **Description:** Checks if a move to the given position `[x, y]` is valid.
- **Parameters:**
  - `x` (int): X-coordinate of the position.
  - `y` (int): Y-coordinate of the position.
- **Returns:** True if the move is valid, False otherwise.

### `explore_path(position: list) -> None`

- **Description:** Recursively explores all possible moves from the given position and saves the valid moves in the path list.
- **Parameters:**
  - `position` (list): Current position `[x, y]`.

### `trim_path() -> None`

- **Description:** Trims the path list to only include positions on the last row, removing additional positions that are not on the last row.

<img src="https://user-images.githubusercontent.com/72719359/169643297-d6ec554b-5980-4c54-8d67-23319763436b.png">
<h3>Contact Me</h3>

<a href="https://t.me/LampStack">Telegram</a><br>
<a href="mailto:xialop@outlook.com">Email</a>

