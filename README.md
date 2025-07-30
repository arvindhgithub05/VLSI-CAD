# VLSI-CAD
Libraries used:
1. Matplotlib for plotting graphs
2. Numpy for performing mathematical functions 
3. Networkx for plotting polar graphs

Objectives:
1. To find a suitable and optimal floorplan for the given set of block dimensions
2. To minimize cost and find the global minima (a point where the cost function is the least) such that the area and wirelengths are meticulously reduced.
3. Use heuristic and greedy algorithms to locate a global minima and thereby select the best design

Flow:
1. For the given polish expression, devise a binary tree using data structures such that these nodes and edges represent the block bordering and connections.
2. For computing routing length, calculate the Manhattan distance between two consecutive blocks using the given expression
3. To compute the area of the entire design, locate the lowest point and the highest coordinate point and derive the height and width of the design.
4. Finally, compute the cost function. This result is a starting point or a seed, which is used as a reference point for optimization
5. To vary the orientation of the blocks, i.e., to find the minimum area and wirelength, perform perturbations to the blocks and observe the least cost design.
6. Polar graphs give a rough idea about the horizontal and vertical connections
7. Using Simulated Annealing, both a greedy algorithm (selects the least cost, but could just be a local minima) and heuristic algorithm (highest chances of finding global minima but computationally intensive), find the best floorplan and select that floorplan as the design output.
