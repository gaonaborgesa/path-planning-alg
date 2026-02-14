# Path Planning Algorithm

> **Note:** This project was originally completed as part of CSC 386 coursework at Berea College. This is a personal copy to showcase my work.

## Overview

Implemented path planning algorithms in C++ for autonomous robot navigation. The system allows a robot to compute optimal paths from its current position to a goal position while navigating around obstacles using graph search algorithms.

## Technical Details

• **Language:** C++  
• **Hardware:** MBot-Omni robot platform  
• **Key Concepts:** Graph search algorithms (BFS, DFS, A*), distance transforms, occupancy grids, optimal path planning  
• **Visualization:** Web-based navigation interface for real-time path visualization

## Implementation

### Graph Search Algorithms

Developed multiple path planning approaches:

• **Breadth-First Search (BFS):** Implemented complete exploration strategy guaranteeing shortest path in unweighted graphs  
• **Depth-First Search (DFS):** Created memory-efficient search for rapid exploration  
• **A* Search:** Designed heuristic-guided optimal path planning with distance transforms  
• **Distance Transform:** Generated collision-aware cost maps for safer navigation around obstacles

### Key Features

• Occupancy grid representation of the environment  
• Multiple maze configurations for testing (simple obstacles, narrow passages, complex mazes)  
• Web app integration for real-time visualization  
• Command-line interface for robot execution  
• Path optimization with collision avoidance

## Technical Challenges Solved

• Converting 2D grid environments into searchable graph structures  
• Implementing efficient graph traversal algorithms  
• Integrating distance transforms for path safety  
• Optimizing pathfinding performance for real-time robot navigation  
• Handling edge cases in narrow passages and complex environments

## What I Learned

• Graph search algorithm implementation and optimization  
• Path planning strategies for autonomous systems  
• Distance transforms and their applications in robotics  
• Real-time visualization and debugging techniques  
• Trade-offs between different search algorithms (completeness, optimality, efficiency)

## Usage

### Compilation

```bash
cd build
cmake -D MBOT=On ..
make
```

### Running on Robot

```bash
./robot_plan_path ~/current.map [goal_x] [goal_y]
```

### Web App Testing

Instructions available at: https://hellorob.org/tutorials/app.html

## Demo

![maze1-demo](https://github.com/user-attachments/assets/a0278296-7ae7-4374-8bc5-51f594b5c2ac)

*Path planning demonstration navigating through a complex maze environment*

GIF created with [ScreenToGif](https://www.screentogif.com/) for Windows

## Project Instructions

Full project specifications available [here](https://hellorob.org/projects/p3).

## License

See [LICENSE.txt](LICENSE.txt) for details.

## Acknowledgments

Project completed as part of CSC 386: Autonomous Systems coursework at Berea College.
