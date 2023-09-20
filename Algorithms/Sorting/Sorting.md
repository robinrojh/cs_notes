---
tags:
  - Sorting
  - Algorithm
---
| Sorting Algorithms                         | Time Complexity      | Space Complexity | Remarks                                                                                                                                                         |
| ------------------------------------------ | -------------------- | ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [BubbleSort](BubbleSort.md)   | n2, n2, n            | 1                | Best when sorted, also when almost sorted eg. [1, 2, 3, 4, 2]<br><br>Invariant: Last few elements sorted (bubble), first few elements sorted (insertion) Stable |
| [InsertionSort](InsertionSort.md) | n2, n2, n            | 1                |                                                                                                                                                                 |
| [SelectionSort](SelectionSort.md)                                  | n2, n2, n2           | 1                | Invariant: last few/first few sorted depending on min/max Unstable                                                                                              |
| [MergeSort](MergeSort.md)                                      | All n log n          | n                | Invariant: each subarray is sorted after the end of each merge<br><br>Stable (if merge is stable)                                                               |
| [Quicksort](Quicksort.md)                                      | n2, n log n, n log n | n                | Invariant: At the end of each iteration, i >= high, A[i] > pivot<br><br>1 < j < low, A[k] < pivot Unstable                                                      |
