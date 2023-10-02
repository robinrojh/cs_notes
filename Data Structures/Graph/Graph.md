---
tags:
  - DataStructure
  - Graph
  - CS2040
---
#### Graph components
1. V: Vertices/nodes
2. E: Edges/lines, may be weighted
3. Can be undirected or directed

#### Simple Graph
1. No loop, no multiple & parallel edges
2. 0 <= # of edges <= O(V<sup>2</sup>)

### Undirected Graph
| Terminology         | Description                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Path                | a group of edges exist in between two nodes                                                                                                                       |
| Simple path         | a path but no repeated vertices along the path                                                                                                                    |
| Connected           | a path exists for every pair of vertices                                                                                                                          |
| Connected component | graph C is a connected graph of graph G if C is a subgraph of G, C is connected, and no connected subgraph of G has C as a subgraph and also other vertices/edges |


### Directed Graph
| Terminology                  | Description                                                           |
| ---------------------------- | --------------------------------------------------------------------- |
| in-degree                    | # of edges pointing into the target node                              |
| out-degree                   | # of edges pointing out from the target node                          |
| Strongly connected component | Path exists from one component to any other component in the same SCC |
| Cycle                        | A path that starts & ends at the same vertex                          |
| Directed Acyclic Graph (DAG) | directed graph that has no cycles                                     |
#### Directory
- [[Tree]]
- [[CompleteGraph]]
- [[BipartiteGraph]]
- [[DirectedAcyclicGraph]]
- [[BreadthFirstSearch]]
- [[DepthFirstSearch]]
- [[MinimumSpanningTree]]
