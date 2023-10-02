---
tags:
  - Algorithm
  - Graph
  - CS2040
---
#### Description:
**Problem: How can I look for a specific element in a graph?**
1. Recursively searches through one branch first before moving onto another
 --> leads into a problem if a cycle is encountered!
2. Keeps a status array to see if a vertex has been visited already
3. Keeps a previous array to track the previous vertices

**Cycle Detection**
1. modify visited array to represent three states:
	1. unvisited
	2. explored
	3. visited, which now means all neighbors of this vertex has been explored

#### Time complexity:
- Best: 
- Average: O(V + E)
- Worst: 

#### Remarks:
- Can be used for SSSP in weighted tree graphs
	- [[SingleSourceShortestPath]]