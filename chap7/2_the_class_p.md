# 7.2 The Class P

##### 定义7.12（P）

$$P=\bigcup\limits_{k}$$TIME$$(n^k)$$.

> $$P$$ is the class of languages that are decidable in polynomial time on a deterministic single-tape Turing machine.

#### P的例子

##### 定理7.14

$$PATH=\{<G,s,t>|G$$ is a directed graph that has a directed path from $$s$$ to $$t\}$$

$$PATH\in P$$

> 判断有向图G中，s点到t点是否可达

##### 定理7.16

Every context-free language is a member of P.

> 因此识别CFL文法的编译器parser总能在多项式时间内完成parse
>
> 证明方法：构造法
