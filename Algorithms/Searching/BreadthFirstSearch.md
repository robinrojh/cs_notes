---
tags:
  - Algorithm
  - Graph
  - CS2040
---
#### Description:
**Problem: How can I look for a specific element in a graph?**
1. Looks for all neighbors before moving onto the next elements
--> keeps a queue to order the visits
2. Keeps a Boolean array of size V to track visited vertices
#### Time complexity:
- Best: 
- Average: O(V + E)
- Worst: 

#### Remarks:
- Can be used to solve unweighted SSSP problem (or in the case where edge weight are all equal)!
	- Change visited array to an integer array D s.t. D\[`u`\]initially for all `u`
	- Set D\[s\] = 0
	- Tweak: for an unvisited vertex v, D\[v\] = D\[u\] + 1
	- [[SingleSourceShortestPath]]