---
tags:
  - Algorithm
  - CS2040
  - CS3230
---
Master theorem is not applicable if:
**T(n) = aT(n/b) + f(n)**
- T(n) is not monotone, ex: T(n) = sin n
- f(n) is not a polynomial, ex: T(n) = 2T(n/2) + 2n
## Master Theorem
### f(n) = a * f(n/b)+ g(n)
### Case 1: Driving function < watershed function
1. a >= 1, b > 1
2. g(n) is asymptotically positive
--> **f(n) = $\theta$(n<sup>log<sub>b</sub>a</sup>)**
Solve recurrence by comparing driving function g(n) to watershed function n<sup>log<sub>b</sub>a</sup> (watershed function = asymptotic number of leaves)
--> if O(n<sup>log<sub>b</sub>a - ε</sup>) for ε > 0, watershed function dominates --> **f(n) = $\theta$(n<sup>log<sub>b</sub>a</sup>)**
### Case 2: $\theta$(n<sup>log<sub>b</sub>a</sup> log<sup>k + 1</sup> n)
**Example: k = 0**
1. a = b
2. watershed = n<sup>log<sub>b</sub>a</sup> = n as a = b
3. driving = f(n) = n

### Case 3: Driving function > watershed function
**Example: f(n) = 4 * f(n/2) + n<sup>3</sup>
1. watershed = n<sup>2</sup>
2. driving = n<sup>3</sup> = $\Omega$(n<sup>2 + ε</sup>), so ε = 1
3. 4 * (n/2)<sup>2</sup> <= c * n<sup>3</sup> for c = 1/2
4. Thus f(n) = $\theta$(n<sup>3</sup>)