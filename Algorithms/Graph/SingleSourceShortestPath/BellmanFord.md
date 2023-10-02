---
tags:
  - Algorithm
  - Graph
  - CS2040
---
#### Description:
**Problem: SSSP
- Does not work with negative cycles!
- Relax every edge one time to make get the shortest distance
```
for i = 1 to |V|-1 // O(V) here, so O(VE * 1) = O(VE)  
  for each edge(u, v) ∈ E // O(E) here, e.g. by using an Edge List  
    relax(u, v, w(u, v)) // O(1) here
```
- Theorem 1: If G = (V, E) contains **no negative weight cycle**, then the shortest path **p** from source vertex **s** to a vertex **v** must be a **simple path**.
- Theorem 2: If G = (V, E) contains **no negative weight cycle**, then after Bellman-Ford algorithm terminates, we will have **D\[u\]** = **δ(s, u)**, ∀ **u** ∈ **V**.
- Can use Bellman Ford to detect negative cycles
#### Time Complexity:
- Best: 
- Average: O(V * E)
- Worst: 

#### Auxiliary Space:
- O(V)
#### Remarks:
