---
tags:
  - DataStructure
---
Name: Chaining structure for hash tables

Description: uses linkedlist in each bucket of the hash table instead of skipping to another bucket in hash table

Space Complexity: O(m + n), where m = table size, n = linkedlist size

| Operations | Time Complexity | Space Complexity |
| ---------- | --------------- | ---------------- |
| insert     | O(log n), O(1)  |                  |
| delete     | O(n)            |                  |
| search     | O(n), O(1)      |                  |

Remarks:
	complexity under Simple Uniform Hashing assumption
	n / m items in each bucket under SUH