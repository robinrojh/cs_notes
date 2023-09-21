---
tags:
  - Algorithm
---
#### Description:
**Problem: MST
- Starts from a source graph and spans through every vertex
- Uses PQ data structure to sort edges by **non-decreasing weight order
- Uses an adjacency list data structure
- Uses a Boolean array to check for cycle (direct addressing table)
1. Start from source `s` and add all edges incident to `s` into the PQ
2. If the first edge in the PQ (smallest weight) has NOT been visited, extend the tree `T` to add the edge into the PQ
#### Time complexity:
- Best: 
- Average: O(E log V)
- Worst: 
1. ExtractMax from PQ = O(log E) = O(log V<sup>2</sup>) = O(2 log V) = O(log V)
2. E edges, so O(E log V)
#### Remarks:
