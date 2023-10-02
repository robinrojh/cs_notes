---
tags:
  - Algorithm
  - CS2040
---
#### Description:
**Problem: find a more efficient way of searching for an element in a sorted array than linear search**

Searches for an element in a sorted array by using divide-and-conquer method.

1. Compare `middle` element with `target`, with pointer `lo` to first index and pointer `hi` to the last index
2. If `target` == `middle`, search complete, return the result
3. If `target` < `middle`, recursive call w/ `hi` to `middle - 1`
4. If `target` > `middle`, recursive call w/ `lo` to `middle + 1`
5. If no answers are found until `lo` >= `hi`, `target` does not exist in the target array
#### Time complexity:
- Best: O(log n)
- Average: O(log n)
- Worst: O(log n)

#### Remarks:
- Only able to use in a **sorted** array!