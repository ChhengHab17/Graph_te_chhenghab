# GRAPH TRAVERSAL

## Graph overview
  Edge list : {0, 1}, {0, 2}, {1, 3}, {1, 4}, {2, 5}, {2, 6}, {3, 5}
## DFS Process and result
Depth-First Search (DFS) explores as deeply as possible along each branch before backtracking. It can be implemented using either recursion or a stack.
DFS Steps:
1. Start at the given node.
2. Mark the node as visited and visit its first unvisited neighbor.
3. Repeat the process for each subsequent neighbor, continuing as deep as possible.
4. Once no unvisited neighbors remain, backtrack to the previous node and visit any remaining unvisited neighbors.
5. Repeat until all nodes are visited.
### Result
0 -> 1 -> 3 -> 5 -> 2 -> 6 -> 4
## BFS Process and result
Breadth-First Search (BFS) explores the graph level by level, visiting all neighbors of a node before moving to the next level.
BFS Steps:
1. Start at the given node.
2. Mark the node as visited and enqueue it into a queue.
3. Dequeue a node from the front of the queue, visit its unvisited neighbors, and enqueue them.
4. Repeat the process until the queue is empty.
### Result
0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6
## Traversal in DFS
The DFS traversal order can vary depending on the adjacency list order (which determines the neighbor visit order). In this case, we observe different DFS orders based on whether we visit 3 or 4 first, and similarly for 5.
## Traversal in BFS
The BFS traversal order remains consistent as it explores level by level. However, BFS results may differ if we have different starting points or graph structures.


