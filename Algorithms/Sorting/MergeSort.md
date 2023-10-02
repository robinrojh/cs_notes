---
tags:
  - Sorting
  - Algorithm
  - CS2040
---
Time Complexity: 
- Worst: O(n log n)
- Average: O(n log n)
- Best: O(n log n)

Space Complexity:
* O(n)

Stability: Stable ONLY IF `merge` is stable

Invariant: Each subarray is sorted after the end of each merge

![[Pasted image 20230917131409.png]]
Merge sort uses **divide and conquer**, typically recursive, approach.
Computationally slower than quicksort in most cases even though the time complexity is better!