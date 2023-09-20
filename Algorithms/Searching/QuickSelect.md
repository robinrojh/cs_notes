---
tags:
  - Algorithm
---
#### Description:
**Problem: Find the k-th smallest element in an UNSORTED array**
1. Partition the array about a pivot
2. The index `i` of the pivot after partitioning is at the right order of sorted array
	1. E.g. if i = 2, `array[i]` = third smallest element in the array
3. Recurse on one side and repeat until k-th smallest element is found.
- Do not need sorting-- only partitioning!
#### Time complexity:
- Best: O(n)
- Average: O(n)
- Worst: O(n)

#### Remarks:
