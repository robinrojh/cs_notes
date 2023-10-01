---
tags:
  - Principle
---
#### Name: Producer Extends, Consumer Super

#### Description:
- If var returns a variable of type T, ? extends T
- If var accepts a variable of type T, ? super T


#### Example:
- ```
```
public <R> InfiniteList<R> map(Transformer<? super T, ? extends R> mapper)
Transformer consumes type T, and returns type R.

public abstract <U> Maybe<U> flatMap(Transformer<? super T, ? extends Maybe<? extends U>> transformer);
```