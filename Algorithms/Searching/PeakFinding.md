---
tags:
  - Algorithm
---
#### Description:
**Problem: Finding a local maximum in an UNSORTED array** 
- `array[i - 1]` <= `peak` <= `array[i + 1]`, where i is the index of the peak
- There is always a local maximum in a given range `[lo:hi]`.
#### Time complexity:
- Best: O(log n)
- Average: O(log n)
- Worst: O(log n)
T(n) = T(n / 2) + $\theta$(1)
#### Remarks:
