---
tags:
  - Algorithm
  - CS3230
---
#### Description:
**Given two decision problems A and B, polynomial-time reduction from A to B (A ≤<sub>p</sub> B) is a transformation from instance a of A to instance b of B.

1. _a_ is a YES-instance for **A** if and only if **b** is a YES-instance for **B**.  
    (A YES-instance is an instance of the decision problem whose answer is YES/True).
2. The transformation takes polynomial time in the size of _a_.
- With a polynomial-time reduction, we will be able to claim that the problem of solving A is only as hard as solving B
- However, B is hard does not imply A is hard, A is "easy" does not mean B is "easy"

- [[CSAT]]
- [[Clique]]