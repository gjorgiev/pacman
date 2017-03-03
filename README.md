# pacman
AI agent playing PACMAN.

Anaconda can be used to run project. The command to create Conda env. is below.
conda create -n pacman python=2

python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic 
python pacman.py -l openMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic 
python pacman.py -l openMaze -z .5 -p SearchAgent -a fn=astar,heuristic=euclideanHeuristic

python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5
python pacman.py -l bigCorners -p AStarCornersAgent -z 0.5

python pacman.py -l trickySearch -p SearchAgent -a fn=ucs,prob=FoodSearchProblem //~16000 nodes are expanded.
vs
python pacman.py -l trickySearch -p AStarFoodSearchAgent // below 7000 nodes are expanded.