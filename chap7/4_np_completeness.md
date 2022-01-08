# 7.4 NP-completeness

1970年，Stephen Cook和Leonid Levin发现有一类问题. If a polynomial time algorithm exists for any of these problems, all peoblems in NP would be polynomial time solvable. 

These problems are called ***NP-complete***.

##### 定理7.27（SAT问题）

$$SAT=\{<\phi>|\phi$$ is a satisfiable Boolean formula$$\}$$.

$$SAT\in P$$ iff P=NP.

> satisfiability problem：布尔表达式是否可能为true
>
> e.g. $$\phi=(x\cap y)\cup(x\cap z)$$

##### 定义7.29（polynomial time reduction）

$$B\leq_PC$$

> 符号可以理解为：在以多项式为粒度的难度方面，$$B\leq C$$，C更（或相同）难

TODO

##### 定义7.34（NP-complete）

A language $$B$$ is ***NP-complete*** if it satisfies two conditions:

1. $$B$$ is in NP, and
2. every $$A$$ in NP is polynomial time reducible to $$B$$

##### 定理7.35（NP-complete和P=NP?的关系）

If $$B$$ is NP-complete and $$B\in P$$, then P=NP.

##### 定理7.36（NP-complete内的等价关系）

If $$B$$ is NP-complete and $$B\leq_PC$$ for $$C$$ in NP, then $$C$$ is NP-complete.

> 再结合NP-complete的定义可知：$$C\leq_PB$$

##### 定理7.37（Cook-Levin定理）

$$SAT$$ is NP-complete.

##### 推论7.42

$$3SAT$$ is NP-complete.

> 证明方法：$$SAT\leq_P3SAT$$
