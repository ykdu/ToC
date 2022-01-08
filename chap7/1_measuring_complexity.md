# 7.1 Measuring Complexity

##### 定义（TIME language集合）

Let $$t:N\rightarrow R^+$$ be a function.

Define the time complexity class, ***TIME(***t(n)***)*** to be the collection of all languages that are decidable by an $$O(t(n))$$ time Turing  machine.

##### 定理7.8（time complexity of multitape TM）

Let $$t(n)$$ be a function, where $$t(n)\leq n$$. Then every $$t(n)$$ time multitape TM has an equivalent $$O(t^2(n))$$ time single-tape Turing machine.

##### 定理7.9（time complexity of nondeterministic TM）

Let $$t(n)$$ be a function, where $$t(n)\leq n$$. Then every $$t(n)$$ time nondeterministic single-tape TM has an equivalent $$2^{O(t(n))}$$ time deterministic single-tape Turing machine.
