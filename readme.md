# Pacman AI

Challenge creditted to UC Berkeley, (http://ai.berkeley.edu) <br/>
Partner: www.github.com/ootmon1

# Introduction

In this project, your Pacman agent will find paths through his maze world, both to reach a
particular location and to collect food efficiently. You will build general search algorithms and
apply them to Pacman scenarios.

# Commands to test the AI:

**Finding a dot with DFS:** <br/>
  python pacman.py -l tinyMaze -p SearchAgent
  python pacman.py -l mediumMaze -p SearchAgent
  python pacman.py -l bigMaze -z .5 -p SearchAgent
  
**Finding a dot with BFS:**<br/>
  python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
  python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5

**UCS:**<br/>
  python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs
  python pacman.py -l mediumDottedMaze -p StayEastSearchAgent
  python pacman.py -l mediumScaryMaze -p StayWestSearchAgent
  
**AStar**:<br/>
  python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic
  
**Finding the 4 corners of the map (BFS):**<br/>
  python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
  python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
 
**Finding the 4 corners of the map (AStar)**:<br/>
  python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5
