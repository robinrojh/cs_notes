---
tags:
  - Principle
  - CS2030
---
#### Name: Variance

#### Description: Covariance, Contravariance, Invariance
- Covariant if S <: T --> C(S) <: C(T)
- Contravariant if S <: T --> C(T) <: C(S)
- Invariant if neither
#### Example:
- #### Covariance
	Integer[] intArray;
	Object[] objArray;
	objArray = intArray; → this is fine as Integer[] <: Object[] (covariant)
```
List<? extends Number> nums = new ArrayList<Integer or Double or Float...>(); 
// Read with Number n = nums.get(k);
```
- #### Contravariance
	- Use ? super T keyword
	- **Cannot safely read anything from this contravariant structure