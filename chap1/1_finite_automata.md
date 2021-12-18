# 1.1 Finite Automata

##### 定义1.5（FA）

A ***finite autamation*** is a 5-tuple $$(Q,\Sigma,\sigma,q_0,F)$$, where

1. $$Q$$ is a finite set called the ***states***,
2. $$\Sigma$$ is a finite set called the ***alphabet***,
3. $$\sigma:Q\times\Sigma\rightarrow Q$$ is the ***transition function***,
4. $$q_0\in Q$$ is the ***start state***,
5. $$F \subseteq Q$$ is the ***set of accept states***

> 状态转移图是描述FA的一种方法，但FA并不总能用图表示（当1.图太大，2.FA的包含变量时），所以不要认为FA就是状态转移图。

##### 定义（FA's computation ）

Let $$M$$ be a FA, and let $$w=w_1w_2...w_n\ (w_i\in\Sigma)$$ be a string. Then $$M$$ ***accepts*** $$w$$ if a sequence of states $$r_0,r_1,...,r_n\ (r_i\in Q)$$ exists with three conditions:

1. $$r_0=q_0$$
2. $$\sigma(r_i,w_{i+1})=r_{i+1}$$, for $$i=0,...,n-1$$
3. $$r_n\in F$$

如果$$A=\{w|M$$accepts $$w\}$$，则称$$M$$ ***recognizes language*** $$A$$

##### 定义1.16（regular language）

A launguage is called a ***regular launguage*** if some finite automaton recognizes it.



##### 如何设计一个FA？

为具体的一种语言设计FA没有固有方法，是一个创作的过程。



NOTE: 字符串、language、机器(automata/machion)



##### 定义1.23（regular operation）

> 以regular language为操作数的集合运算符称为regular operation。

Let $$A$$ and $$B$$ be languages. We define three regular operations as follows:

- ***Union***: $$A\cup B=\{x|x\in A or x\in B\}$$
- ***Concatenation***: $$A\cdot B=\{xy|x\in A\ and y\in B\}$$
- ***Star***: $$A^*=\{x_1x_2...x_k|k\ge 0$$ and each $$x_i\in A\}$$

##### 定理（regular languages的封闭性）

The class of regular languages is closed under the Union, Concatenation and Star operation

> 证明方法：通过NFA+构造法
>
> 如果$$A$$和$$B$$是两个regular language，则$$A\cup B$$, $$A\cdot B$$和$$A^*$$依然是regular language
