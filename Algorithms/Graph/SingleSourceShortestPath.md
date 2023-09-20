---
tags:
  - Algorithm
---
#### Description:
**Problem: Find the shortest path from a single source to each vertex in the graph**
Input: 
1. Directed weighted graph G(V, E)
2. A single source vertex v such that v ∈ V

### Operations:
![[Pasted image 20230920100735.png]]

| Operation | Description                                                                                   | Time Complexity | Space Complexity |
| --------- | --------------------------------------------------------------------------------------------- | --------------- | ---------------- |
| Relax     | if path can be shortened, change the distance to that vertex and remember the new predecessor |                 |                  |

#### Faster than Bellman-Ford:
1. On Unweighted Graphs: O(**V**+**E**) BFS,
2. On Graphs without negative weight: O((**V**+**E**) log **V**) Dijkstra's algorithm,
3. On Graphs without negative weight cycle: O((**V**+**E**) log **V**) Modified Dijkstra's,
4. On Tree: O(**V**+**E**) DFS/BFS,
5. On Directed Acyclic Graphs (DAG): O(**V**+**E**) Dynamic Programming (DP)
#### Remarks:
1. [[BellmanFord]]
2. [[Dijkstra]]
3. [[ModifiedDijkstra]]
4. [[BreadthFirstSearch]]
5. [[DepthFirstSearch]]
6. [[DynamicProgramming]]