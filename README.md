# MazeSolver

MazeSolver is a Python class that finds an optimal path through a maze, collecting coins along the way. The goal is to reach the last row while avoiding obstacles (value 1) and collecting coins (value 2).

## Introduction

This Python class, `MazeSolver`, is created to navigate through a maze and collect coins. The algorithm uses recursive depth-first search to explore possible paths and tracks the collected coins.

## Features

- Finds a valid path in a maze.
- Collects coins while navigating through the maze.
- Simple and easy-to-understand implementation.

## Usage

To use the Maze Solver, simply instantiate the `MazeSolver` class with a 2D matrix representing the maze. The valid path and collected coins will be accessible through the `path` and `coins` attributes.

```python
maze_input = [
    [0, 1, 1, 1, 1],
    [0, 0, 0, 2, 1],
    [1, 0, 1, 1, 1],
    [1, 0, 0, 2, 0]
]

solver = MazeSolver(maze_input)
print("Valid Path:", solver.path)
print("Collected Coins:", solver.coins)
```

<img src="https://user-images.githubusercontent.com/72719359/169643297-d6ec554b-5980-4c54-8d67-23319763436b.png">
<h3>Contact Me</h3>

<a href="https://t.me/LampStack">Telegram</a><br>
<a href="mailto:xialop@outlook.com">Email</a>

