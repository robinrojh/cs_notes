---
tags:
  - Sorting
  - Algorithm
---
Time Complexity: 
- Worst: O(n<sup>2</sup>)
- Average: O(n log n)
- Best: O(n log n)

Space Complexity:
* O(n)

Stability: unstable, but stable algorithms exist

Invariant: At the end of each iteration:
* i >= high
* A[i] > pivot, 1 < j < low, A[k] < pivot

Typically fast
There are many algorithms that improves quicksort:
1. [3-way Quicksort](/Algorithms/Sorting/Quicksort/3-WayQuicksort.md)
2. [Pivot](Pivot.md)