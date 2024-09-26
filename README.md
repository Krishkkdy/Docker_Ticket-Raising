Autobot Warehouse Simulation
Description
This Python-based simulation visualizes autonomous bots navigating through a warehouse environment using the A* pathfinding algorithm. The program allows users to dynamically set obstacles, start points, and end points within a customizable grid. The GUI, built with Tkinter, offers interactive elements to configure the simulation environment, providing real-time visual feedback on the bot movements.

Prerequisites
Python: The application is developed and tested in Python 3.8. Ensure that Python 3.x is installed on your machine.
Tkinter: This GUI toolkit is bundled with most Python installations. If it is missing, it can be installed via pip:
bash
Copy code
pip install tk
Installation
No additional installation is required beyond having Python and Tkinter. Simply download the script or clone the repository containing the project files to your local machine.

Running the Program
Launch the Program:

Navigate to the directory containing the script.
Run the script through the command line:
bash
Copy code
python autobot_simulation.py
Replace autobot_simulation.py with your script's filename if different.
Initialize the Grid:

A dialog box will prompt you to enter the grid size when the program starts. Input an integer value (e.g., 5 for a 5x5 grid) within the permissible range of 2 to 20.
Configure the Simulation:

The main GUI window displays a grid based on the specified size.
Placing Obstacles: Click the "Place Obstacles" button, then click on any grid cell to mark it as an obstacle, which will appear in red.
Adding Bots: Click the "+Bot" button to initiate the placement of a new bot:
First click defines the start position (green cell).
Second click sets the end position (yellow cell).
Repeat the above steps as needed to place multiple bots.
Run the Simulation:

Once all bots and obstacles are placed, click "Start Simulation". The program will simulate each bot's journey from start to end, avoiding obstacles, with each bot displayed in a distinct color.
The movement of bots is animated in the grid, showing a step-by-step traversal based on the calculated path.
Additional Controls:

Clear Grid: Resets the entire grid, removing all bots, obstacles, and paths.
Close: Exits the program.
Features
Interactive Grid Setup: Users can interactively place obstacles and define paths for multiple bots within the grid.
A Algorithm Implementation*: The program utilizes the A* search algorithm to determine the shortest path for each bot from its start to its end point, considering obstacles.
Real-Time Visualization: Each step of the bot's path is visualized in real-time, allowing users to visually track the pathfinding process.
Multiple Bots: Supports configuring and running simulations for multiple bots simultaneously.
Troubleshooting
Ensure all start and end positions are paired correctly; the simulation will not start if there is an unequal number of starts and ends.
If the grid does not respond to clicks, ensure that the program window is active and not minimized.
