---
tags:
  - DataStructure
  - CS2040
---
Name: Fingerprint Hash Table

Description: 
* Does not store key in table, and no false negatives
→ you can always correctly search for values alr in table
* But false positives
→ may return true for searching values not in the table
→ at most 1 - (1 / e)<sup>n/m</sup> probability of false positive
n / m <= 1/2 log (1 / (1 - p<sup>1/2</sup>))

| Operations | Time Complexity | Space Complexity |
| ---------- | --------------- | ---------------- |
|            |                 |                  |

Remarks: