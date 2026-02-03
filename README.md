# Pacman Search Algorithms
<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/450dbc0e-91e5-4356-95cc-f528effa0aff" />

## Overview
This project implements AI search techniques in **Python** to guide Pacman through complex maze environments. The work focuses on designing search problem formulations and applying classical algorithms to find efficient paths for collecting food while minimizing path cost.

## Key Objectives
- Model maze navigation and food collection as formal search problems
- Compute efficient paths using **BFS** and **A\*** with admissible heuristics
- Handle large state spaces using an approximation strategy when optimal search is too expensive

## What I Implemented
### Search Problem Design
- Defined **state representations** to capture Pacman’s position (and food state when needed)
- Implemented **successor functions** to generate valid next states and action costs
- Implemented **goal tests** for completing tasks (e.g., reaching targets, collecting all food)

### Algorithms
- **Breadth-First Search (BFS)**  
  Used for shortest-path solutions in unweighted settings where exploring uniformly by depth is effective.
- **A\* Search**  
  Implemented A\* to reduce search time using **admissible heuristics** while guaranteeing optimality.
- **Greedy Approximation Strategy**  
  Developed a greedy approach for scenarios with very large state spaces (e.g., collecting all food) where optimal search becomes computationally expensive.

## Results
- Efficiently navigates Pacman through mazes using systematic search
- Uses heuristics to significantly reduce explored nodes in A\*
- Scales better on large problems by switching to approximation when needed

## Tech Stack
- **Language:** Python  
- **Concepts:** Search problems, BFS, A\*, admissible heuristics, approximation strategies

## How It Works (High Level)
1. Encode the maze task as a search problem (state, actions, transitions, goal)
2. Run BFS or A\* depending on the problem constraints
3. For large food-collection tasks, apply a greedy strategy to produce a near-optimal solution quickly

## Skills Demonstrated
- AI search and heuristic design
- Problem formulation (state space modeling)
- Efficient algorithm implementation in Python
- Trade-offs between optimal and approximate solutions
