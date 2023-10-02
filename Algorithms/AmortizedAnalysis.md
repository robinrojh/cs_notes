---
tags:
  - Algorithm
  - CS3230
---
#### Description:
Analysis of average performance of each operation

### Methods for Amortized Analysis
#### **Aggregate
- Counting out the cost for each operation
- At the end, show that the average cost is T(n) / n time!
- Example: dynamic table (occasionally increases/decreases table size when push/pop)

#### **Accounting
- Assign charge to each amortized operation, named amortized cost
- The charge may be less than or more than the amortized cost
- If the amortized cost is less than the actual cost, the rest are saved as a "credit"
#### Potential
- Similar to accounting
- Associate a potential function Φ with algorithm/data structure
	Φ(i) = potential at the end of ith operation
	Φ(i) >= 0 for ALL i
	Amortized cost of ith operation = actual cost of ith operation + (Φ(i) - Φ(i - 1))
	If high cost, then delta Φ(i) will be negative and will mitigate the impact of high cost
	If low cost, then delta Φ(i) will be positive
	Amortized cost of n operations >= actual cost of n operations - Φ(0)
**![](https://lh6.googleusercontent.com/hGGj4X7_oYKXBa0yQMvs6Lf09R4LaePGqs66hrN7Ydmibol8-eEpr2VGuM4jSIy7t6W7sgQ-P6uP3s7ECJwBiKq4yVbi3bP681iNmsdEktP2XH0idGgIagHmJZMa57MT8NBH09k0Y3AoXSd2CwOb-A)**
