# SafeStar
 ME570: Robot Motion Planning Final Project. An implementation of modified A* Algorithm path planning for escaping active shooter scenaiors

## Required Packages:
* numpy
* pygame

## User Instructions
To generate the figures see the comments in main_results.py reproduced below:

Pygame creates one figure at a time because it runs until the user exits.

In order to generate a figure that is used in the report, find the appropriate section (see lines 46 through 177 of draw_visualization.py) and comment out all but one of the figure's variables and run the script. It will generate the figure with the specified input parameters.

In order to generate your own figures, use the following guide below for the appropriate inputs. See graph.py for more details about each specific parameter and function.

If you have any questions, please feel free to contact me at ianjchadwick@gmail.com or ianjc@bu.edu


To use with Safe* and A* search:
 Inputs:
 size: an integer for the (square) grid side length
 obstacles: a list of coordinates describing the shape of obstacles in the format (from top left) 
            [[topleftx, toplefty], verticalheightdown = int, horizontal_width_right = int]
 exits = List of [x,y] coordinates of exit(s)
 shooters = List of [x,y] coordinates of shooter(s)
 start = [x,y] coordinate of start location
 
 Output:
 The grid with:
  Obstacle/blocked squares marked in black.
  Shooter Location(s) marked in red.
  Start Location marked in blue.
  Exit(s) marked in green.
  The Safe* Path is marked in purple.
  The A* Path is marked in orange. (in the case they share the same square Safe* is colored over by A*)

## Algorithm Explanation
See the final paper in the documents folder for details about the algorithm.
