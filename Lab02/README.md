# **Rescue Mission Game**

## **Overview**

The Rescue Mission Game is a grid-based game where the objective is to navigate from a starting point (`S`) to rescue a trapped character (`R`). The grid also contains obstacles (`X`) that block the player's path. The game uses the A\* algorithm to find the shortest path from the starting point to the trapped character while avoiding obstacles.

## **Features**

* **Grid Creation:** Generates a grid with a user-defined size and randomly places a trapped character and obstacles.  
* *A Pathfinding:*\* Implements the A\* algorithm to calculate the shortest path to the trapped character.  
* **Modular Code:** Structured to allow easy modifications for different game scenarios.

## **How to Run**

**Clone the Repository:**  
bash  
Copy code  
`git clone https://github.com/yourusername/rescue-mission-game.git`

1. 

**Navigate to the Project Directory:**  
bash  
Copy code  
`cd rescue-mission-game`

2. 

**Run the Game:**  
bash  
Copy code  
`python rescue_mission_game.py`

3. Follow the prompts to enter the grid size and number of obstacles.

## **Code Structure**

* `create_grid(size)`: Creates the grid and places the trapped character (`R`).  
* `add_obstacles(grid, num_obstacles)`: Adds obstacles (`X`) to the grid.  
* `is_valid_position(grid, x, y)`: Checks if a position is within bounds and not blocked.  
* `heuristic(a, b)`: Calculates the heuristic for A\* (Euclidean distance).  
* `a_star(grid, start, goal)`: Finds the shortest path using the A\* algorithm.  
* `print_grid_with_path(grid, path)`: Prints the grid with the path marked.  
* `rescue_mission()`: Main function to start the game.

## **Example Output**

mathematica  
Copy code  
`Enter the grid size (e.g., 6 for a 6x6 grid): 6`  
`Enter the number of obstacles (less than 34): 10`

`Initial Grid:`  
`| S |   |   |   |   |   |`  
`|   | X |   |   | X |   |`  
`|   |   | X |   |   |   |`  
`|   |   |   | X |   |   |`  
`|   |   |   |   |   |   |`  
`|   |   | X |   |   | R |`

`Searching for the trapped character using A* algorithm...`

`Path to the Trapped Character:`  
`| S | * | * | * | * | * |`  
`| * | X | X | * | X | * |`  
`| * | * | X | * | * | * |`  
`| * | * | * | X | * | * |`  
`| * | * | * | * | * | * |`  
`| * | * | X | * | * | R |`  
