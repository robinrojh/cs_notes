---
tags:
  - DataStructure
  - Graph
---
#### Name: Union Find Disjoint Set (UFDS)

#### Description: 
**Problem: how can we efficiently determine which set an item belongs to, test if two items belong in the same set, and union two disjoint sets into one?

Options for this DS:
1. Array p of size N where `p[i]` denotes the parent of item i, and if `p[i]` = i, i is the root
	1. another array `rank` where `rank[i]` = upper bound of the height of the subtree rooted at vertex i (guiding heuristic for unionSet(i, j))
2. 

| Operations      | Time Complexity | Space Complexity | Description                                                                                                                                      |
| --------------- | --------------- | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| FindSet(i)      | O(1), O(α(n))   |                  | from vertex i, go up until the root; uses path compression heuristic to point directly to the root                                               |
| IsSameSet(i, j) | O(1), O(α(n))   |                  | checks if FindSet(i) === FindSet(j)                                                                                                              |
| UnionSet(i, j)  | O(1), O(α(n))   |                  | if i and j comes from different disjoint sets, we link the representative item of the shorter tree to the representative item of the taller tree |

#### Remarks:
- α(n) = Inverse Ackermann function