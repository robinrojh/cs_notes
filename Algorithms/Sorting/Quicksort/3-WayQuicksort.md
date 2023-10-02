---
tags:
  - Sorting
  - Algorithm
  - CS2040
---
Time Complexity: 
- Worst: O(n<sup>2</sup>)
- Average: O(n log n)
- Best: O(n) | if all are equal keys

Space Complexity:
* O(log n)

Stability: unstable, but stable implementations exist

Invariant: 

In 3 Way QuickSort, an array arr[l..r] is divided in 3 parts:
1. arr[l..i] elements less than pivot.
2. arr[i+1..j-1] elements equal to pivot.
3. arr[j..r] elements greater than pivot.
![[Pasted image 20230917132656.png]]
