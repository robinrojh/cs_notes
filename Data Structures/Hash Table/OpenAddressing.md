---
tags:
  - DataStructure
  - CS2040
---
Linear Probing: i=(base + step*1) % M,  
Quadratic Probing: i=(base + step * step) % M, and  
Double Hashing: i=(base + step * secondary) % M.

## Primary Clustering

- Formation of long cluster that makes the operations O(n) instead of O(1)
## Secondary Clustering

- Repetition of a pattern when resolving collision, leading to worse time complexity than advertised

## Ways to Prevent Clustering

#### Name: Linear Probing

Description: when a collision is detected, find the next empty/deleted slot and put it there
* load factor α = n / m (< 1)
* expected time to search/insert/delete < 1/(1 – α)

| Operations | Time Complexity | Space Complexity | remarks                                                                                             |
| ---------- | --------------- | ---------------- | --------------------------------------------------------------------------------------------------- |
| insert     | O(1)            |                  |                                                                                                     |
| delete     | O(1)            |                  | instead of actually deleting the value, we put a tombstone value to represent the value as deleted. |
| search     | O(1)            |                  |                                                                                                     |
| resize     | O(n)            |                  |                                                                                                     |

#### Name: Quadratic Probing

Description: when a collision is detected, find the next free slot by incrementing the address
* Attempt 1: h(v) = address --> not free!
* Attempt 2: (h(v) + 1 * 1) % M --> not free
* Attempt 3: (h(v) + 2 * 2) % M --> no collision, so put it in this address!
* **M = hash table size**
* Do **NOT** confuse this with doing h(v), (h(v)+1) % M, (h(v)+1+4) % M, (h(v)+1+4+9) % M

| Operations | Time Complexity | Space Complexity |
| ---------- | --------------- | ---------------- |
|            |                 |                  |

Remarks:
* Main issue-- may cycle forever!
	* If α < 0.5 & M is a prime > 3, we can always find an empty slot
	* --> proof by contradiction
	* Step 1: h(v) + x * x = h(v) + y * y (mod M)
	* Try from here!

#### Name: Double Hashing

Description: to reduce clustering, instead of using step * step, use step * h<sub>2</sub>(v), which is a secondary hash function

| Operations | Time Complexity | Space Complexity |
| ---------- | --------------- | ---------------- |
|            |                 |                  |

Remarks:
1. When will double hashing become the same as Linear Probing?
2. Usually, h<sub>2</sub>(v) = M' - v % M' where M' < M
3. Take into account the hashing function when considering complexities!