# SafeStar  
**ME570: Robot Motion Planning Final Project**  
An implementation of a **modified A\* algorithm** for dynamic **path planning in emergency evacuations**.  

## Overview  
SafeStar is a **motion planning algorithm** that extends A\* search with **safety heuristics**, optimizing escape routes in high-risk environments. The algorithm determines the best path for an individual to reach safety while avoiding hazards.  

## Required Packages  
- `numpy`  
- `pygame`  

## User Instructions  
To generate the figures, refer to the comments in `main_results.py`.  

### Generating Figures  
1. **Visualizing Report Figures**  
   - Locate **lines 46-177** in `draw_visualization.py`.  
   - Comment out all but one relevant figure variable.  
   - Run the script to generate the specified figure.  

2. **Creating Custom Simulations**  
   - Modify the input parameters to test different grid layouts and scenarios.  

### Inputs & Outputs  
- **Inputs:**  
  - `size`: Integer defining the grid size (square dimensions).  
  - `obstacles`: List of **[x, y] coordinates** describing obstacles.  
  - `exits`: List of **[x, y] coordinates** for safe exits.  
  - `hazards`: List of **[x, y] coordinates** for dynamically moving threats.  
  - `start`: **[x, y] coordinate** of the initial position.  

- **Outputs:**  
  The grid visualization will display:  
  - **Obstacles** (black).  
  - **Hazards** (red).  
  - **Start Location** (blue).  
  - **Exits** (green).  
  - **SafeStar Path** (purple).  
  - **A\* Path** (orange). (If overlapping, A\* will overwrite SafeStar.)  

## Algorithm Explanation  
SafeStar integrates a **potential field-based control scheme** with **A\* path planning** to optimize safe egress in dynamic environments.  

For details about the algorithm and mathematical formulation, refer to the **final paper** in the `documents` folder.  
