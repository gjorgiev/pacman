# pacman
AI agent playing PACMAN.

Anaconda can be used to run project. The command to create Conda env. is below.
conda create -n pacman python=2

python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic 
python pacman.py -l openMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic 
python pacman.py -l openMaze -z .5 -p SearchAgent -a fn=astar,heuristic=euclideanHeuristic 