---
tags:
  - DataStructure
  - Topic
  - CS2040
---
#### Name: Adjacency Matrix

#### Description: 
1. has a square matrix of space O(V * V)
2. `matrix[v][w]`shows the weight from vertex v to vertex w, and 0 or -1 to represent no edges

Space Complexity: O(V<sup>2</sup>) 

| Operations     | Time Complexity | Space Complexity |
| -------------- | --------------- | ---------------- |
| count vertices |                 |                  |
| count edges    |                 |                  |
| neighbors      |                 |                  |
| path exists?   |                 |                  |
#### Remarks:


#### Name: Adjacency List

#### Description: 
1. Array of V lists, one index for each vertex
2. Undirected graph: store neighbors of vertex v in list
3. Weighted graph: store neighbor, weight pair in the list

Space Complexity: O(V + E) 

| Operations     | Time Complexity | Space Complexity |
| -------------- | --------------- | ---------------- |
| count vertices |                 |                  |
| count edges    |                 |                  |
| neighbors      |                 |                  |
| path exists?   |                 |                  |
#### Remarks:


#### Name: Edge List

#### Description: 
1. Collection of edges with both connecting vertices and their weights
2. Usually sorted by increasing weight

Space Complexity: O(E) 

| Operations     | Time Complexity | Space Complexity |
| -------------- | --------------- | ---------------- |
| count vertices |                 |                  |
| count edges    |                 |                  |
| neighbors      |                 |                  |
| path exists?   |                 |                  |
#### Remarks:
1. MST Problem