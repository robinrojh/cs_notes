---
tags:
  - Algorithm
  - Graph
  - CS2040
---
#### Description:
**Problem: MST
- Greedy algorithm
- grows a forest of MSTs, eventually combining them
- Makes use of [[UnionFindDisjointSet]] and a good sorting algorithm with edge list

1. Sort the set of edges in a non-decreasing weight order
2. For each edge in the sorted set, greedily take the next edge `e` s.t. `e` does not create any cycles (using UFDS data structure)

#### Loop Invariant: Every edge `e` added to tree `T` must be a part of the MST
- T = {} is an MST
- Checks if adding an edge forms a cycle
#### Time complexity:
- Best: 
- Average: O(E log V)
- Worst: 
1. Sorting edges = O(E log E) from edge list data structure = O(E log V)
2. O(E) union-find disjoint set when calling `isSameSet(u, v)` and `unionSet(u, v)`
	1. O(1) in relatively small graphs
#### Remarks:
