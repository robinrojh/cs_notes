---
tags:
  - DataStructure
  - BST
  - Graph
  - CS2040
---
Name: Scapegoat Tree

Description: Self balancing tree
height is managed based on alpha value: height <= log<sub>1/alpha</sub>(size) + 1
Rebuilds the subtrees after insertion and deletion, so mostly it's O(log n), but in cases of rebuilding it can be O(n)

Space complexity: O(n)

| Operations  | Time Complexity      | Space Complexity |
| ----------- | -------------------- | ---------------- |
| insert      | O(log n)   amortized |                  |
| delete      | O(log n)   amortized |                  |
| search      | O(log n)             |                  |
| traversal   | O(log n)             |                  |
| rotate      | O(log n)             |                  |
| predecessor | O(log n)             |                  |
| successor   | O(log n)             |                  |


Remarks:
Rebuilding:
* Converting each subtree into the most balanced version