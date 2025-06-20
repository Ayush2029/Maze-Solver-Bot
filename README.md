# Maze-Solver-Bot
This is a web-based application that simulates a maze-solving robot. It dynamically generates mazes and visualizes how different pathfinding algorithms (Breadth-First Search, Depth-First Search, and A* Search) navigate through them. The "robot" animates its path, and the application also highlights the cells explored by each algorithm during its search.

<h3> Features: </h3>
- Customizable Grid Size: Users can specify the size of the square maze (must be an odd number greater than or equal to 5). <br>
- User-Defined Start & End Points: <br>
(1) Start Point: Must be one of the specific "corner" cells (e.g., (0,1), (0, Size-2), (Size-2,0), or (Size-2, Size-1)). <br>
(2) End Point: Can be any valid cell within the maze grid. <br>
- Dynamic Maze Generation: Generates a random maze ensuring a valid path always exists from the start to the end point. <br>
- Multiple Pathfinding Algorithms: <br>
(1) Breadth-First Search (BFS): Guarantees the shortest path. <br>
(2) Depth-First Search (DFS): Explores deeply, does not guarantee the shortest path. <br>
(3) A* Search: An informed search algorithm that uses a heuristic to find the shortest path efficiently. <br>
- Animated Path Visualization: A small "robot" (blue circle) animates its movement along the calculated path. <br>
- Explored Path Visualization: Cells visited by the algorithm during its search (but not necessarily part of the final path) are highlighted in light purple, offering insight into each algorithm's search pattern.<br>
- Adjustable Animation Speed: A slider allows users to control the speed of the animation. <br>
- Performance Metrics: Displays the length of the found path, the number of cells explored, and the time taken for each algorithm to find the path. <br>

<h3> How to Use: </h3>
- Download: Clone or download the mazeSolver.html file. <br>
- Open in Browser: Open the mazeSolver.html file directly in any modern web browser (e.g., Chrome, Firefox, Edge). <br>
- Set Grid Size: Enter your desired odd number for the "Grid Size" (e.g., 21, 51, 101). <br>
- Set Start & End Points: Input the row and column coordinates for your desired start and end points. Remember the start point restrictions. <br>
- Generate Maze: Click the "Generate New Maze" button to create a maze with your specified dimensions and points. <br>
- Solve Maze: Choose a pathfinding algorithm (BFS, DFS, or A*) by clicking its respective button. Observe the search exploration and the robot's movement. <br>
- Adjust Speed: Use the "Animation Speed" slider to make the robot move faster or slower. <br>
- Clear Path: Click "Clear Path" to remove the visualizations and see the original maze grid. <br>

<h3> Algorithms Explained: </h3>
- BFS (Breadth-First Search): Explores the maze layer by layer, expanding outwards from the start node. It's guaranteed to find the shortest path in an unweighted graph (like this maze). <br>
- DFS (Depth-First Search): Explores as far as possible along each branch before backtracking. It's not guaranteed to find the shortest path but can be faster if the target is found early on a deep branch. <br>
- A* Search: A more intelligent search algorithm that uses a "heuristic" (in this case, Manhattan distance to the end point) to prioritize which cells to explore next. This often makes it significantly faster than BFS for larger mazes while still guaranteeing the shortest path. <br>

<h3> Technologies Used: </h3>
- HTML5: For the basic structure of the web application. <br>
- CSS3: For styling the layout, buttons, and visual elements, ensuring a responsive and modern user interface. <br>
- JavaScript: For the core logic including maze generation, pathfinding algorithms, and canvas rendering/animation. <br>
- HTML Canvas API: For drawing the maze, explored paths, and the animated robot. <br>

<h3> Conceptual Image Processing: </h3>
While this project is purely software-based for visualization, in a real-world "maze solver robot," image processing would be a critical initial step. A robot's camera would capture the physical maze, and image processing techniques (like thresholding, edge detection, and contour analysis) would be used to: <br>
(1) Map the Maze: Convert the visual information into a digital grid representation (walls vs. paths). <br>
(2) Localize the Robot: Determine the robot's current position within that digital grid. <br>
This application directly uses the digital grid, simulating the output of such an image processing pipeline. <br>
