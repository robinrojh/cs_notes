---
tags:
  - Algorithm
  - Graph
---
#### Description:
**Problem: SSSP 
- Must have no negative weight edges **at all**! **∀ edge(u, v) ∈ E**, **w(u, v) ≥ 0**.
- Maintains a set S of solved vertices (known shortest distances)
	- Initially, S = {source s}
- Then, repeatedly select a vertex u in pq = {V \\ S}
#### Time complexity:
- Best: 
- Average: O((V + E) log V)
- Worst: 
1. V vertices, E edges
2. ExtractMin() used for extracting minimum value from PQ (uses binary min heap or balanced BST) is O(log V)
--> O(V log V)
3. E edges are relaxed as the neighbors are relaxed with every vertex
4. Call DecreaseKey() from binary min heap or delete and insert again in balanced BST, so O(log V)
--> O(E log V)
5. O(V log V + E log V) = O((V + E) log V)
#### Remarks:
- 
