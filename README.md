# Route-Visualizer
Path-finding algorithms are the algorithms that are used to find the shortest path or the shortest route between two points. It will be a visualization tool for various pathfinding algorithms and will have configurations to play around with. The major motivation behind this project is that humans tend to remember visual things more than any other thing. Also, this project could be a good way to teach ourselves about the various path-finding algorithms.

#### Key Features of the project:
1. Our projects use a variety of Algorithms, including `A*`, `Beam Search`, `Best First Search`, `BFS`, `DFS`, `Dijkstra`, `Dynamic A*`, `IDA*`, `Jump Point Search`, `Static A*`, and `Uniform Cost Search` to find a path between two nodes in a graph and the shortest path,i.e, finding the optimal shortest path.
1. The pathfinder has three Modes -  
   • Multiple sources in which all sources simultaneously start their search for the destination, and the final path is drawn from the first source that reaches it.  
   • Multiple destinations, i.e. The source ends its search at the first destination it reaches. The algorithm is guided with the lowest heuristic value from all destinations.  
   • Checkpoints are points that are visited in order by the path from the source to the destination.
1. There are various Configurations available, some of which are Cut corners that prevent the path from touching the corners of obstacle cells during diagonal movement, Allow diagonals that specify whether a diagonal movement is allowed or not, and Bidirectional which specify whether the destination is a moving agent or not.
1. Random mazes are one of the features of the pathfinder, which has 2 maze generation algorithms. Both generate a random maze with a possible path between the two cells. 
1. Wormholes are agents that step on a cell marked as the wormhole entry; it moves to the wormhole exit with 0 costs. The cell marked as a wormhole entry can be considered disconnected from its physical neighbours, and its only neighbour becomes the wormhole exit.
1. Obstacles are cells over which an agent cannot travel. We create a boundary of obstacles around the grid so that the algorithms are bound to the visible screen.


## Guide
First, make sure FLASK is installed on the system:
`pip install flask`

Then, to run the project:-

***For Windows Command Prompt:***
```
    cd Route-Visualizer/src
    set FLASK_APP=api
    flask run
```

***For Windows PowerShell:***
```
    cd Route-Visualizer/src
    $env:FLASK_APP = "api"
    flask run
```

***For Linux / Mac Terminal:***
```
    cd Route-Visualizer/src
    export FLASK_APP=api
    flask run
```
