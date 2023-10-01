---
tags:
  - Principle
---
#### Name: Liskov Substitution Principle (LSP)

#### Description:
Subclass overridden methods should have the same property as the superclass methods.
- Therefore, you should be able to replace the superclass with a subclass

#### Example:
Eg. A extends B
1. A has a method foo() that returns "YES" or "NO"
2. B overrides foo() and this returns "HELLO" or "BYE"
3. B returns an answer that is not in the result set of A, so this violates LSP