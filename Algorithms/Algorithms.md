---
tags:
  - Algorithm
  - Topic
  - CS2040
  - CS3230
---
#### Correctness & Efficiency
- In an algorithm, we want both!
- ***Correct*** if for every input x the algorithm gives a correct answer = worst-case correctness
	- Initialization: invariant is true before the first iteration?
	- Maintenance: invariant is true after the first iterations?
	- Termination: invariant is true after termination and provides useful information?
- ***Efficient*** if scales well with the size of input 
	- Maximum number of steps when run on an input size of n
	- → each step is determined by a computational model

#### Factors to determining a good algorithm
1. Simplicity
2. Space
3. Energy consumption
4. Parallelism
5. Fairness and Ethics

#### Adversarial Argument
- ***Usage:*** prove lower bounds for the running time in concrete computational model
- If algorithm takes too few steps, then it cannot differentiate between two inputs that have different solutions
- Example: query model, comparison model

CS2040S
- [[Sorting]]
- [[Searches]]
- [[Recurrence]]
- [[Reduction]]

CS3230
- [[AsymptoticAnalysis]]