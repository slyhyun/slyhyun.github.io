---
title: Artificial Intelligence Project 1
date: 2024-03-01
all_day: true
---

The project to implement a route finding program using an A* algorithm

<!--more-->
```
1. Overview
This Python program uses the pygame library to visualize the A* path finding algorithm. It helps you understand how the algorithm finds the shortest path between two points, avoiding obstacles on the grid.

2. Initialize and Set Up
- PiGame Initialization: Set the environment for the graphical interface.
- Window settings: Create a window with a size of 900x700 pixels.
- Color definition: Defines the color used for visualization.

3. Set Grid, Obstacle, and Starting Point and Target Point
- Grid definition: defines the play area of 30x30 cells, each of which can be free space or an obstacle.
- Start point and target point: represented by S (start point), G (go point), and can be moved by mouse drag. S and G and obstacles cannot overlap each other.
- Placement of Obstacles : Press the Random Walls button to randomly place obstacles in 20% of the grid. You can use mouse clicks and mouse drag rolls to install and delete obstacles.

4. Implementing Algorithm A*
- Node class : represents each grid cell and has properties (cost, heuristic, total) for managing the A* algorithm.
- Heuristic function: Calculates the estimated cost from the current cell to the target cell in Manhattan distance or Euclidean distance.
- A* Algorithm (astar) : Manage open and closed lists of nodes, and use the minimum heap to extend the path of the lowest cost.

5. Visualization and Interaction
-Draw functions:
-draw_grid : Visualizes the grid, displays free cells, obstacles, start and target cells.
-draw_path : Highlight the path found by A*.
-Button : Start the path finding through the Start A* Search button, change the obstacle configuration through the Random Walls button, and reset the grid through the Reset button. -ratio button : You can choose between Manhattan and Euclidan, respectively.

6. Main Loop
- Continue to check for events and update the screen appropriately.
- Finding a path can be executed by clicking on the specified button area, and the path found (or best attempt if a complete path is not found) is displayed.
```