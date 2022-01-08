# 2.2 Pushdown Automata

图示2.11 2.12：PDA = FA + stack

deterministic PDA跟nondeterministic PDA不等价了，PDA指后者。

##### 定义2.13（PDA）

A ***pushdown automaton*** is a 6-tuple $$(Q,\Sigma,\Gamma,\sigma,q_0,F)$$, where $$Q$$, $$\Sigma$$, $$\Gamma$$, and $$F$$ are all finite sets, and

1. $$Q$$ is the set of states,
2. $$\Sigma$$ is the input alphabet,
3. $$\Gamma$$ is the stack alphabet,
4. $$\sigma:Q\times \Sigma_\epsilon \times\Gamma_\epsilon\rightarrow P(Q\times \Gamma_\epsilon)$$ is the transition function
5. $$q_0\in Q$$ is the start state, and
6. $$F\subseteq Q$$ is the set of accept states.

##### 定义（PDA's computation ）

A pushdown automaton $$M=(Q,\Sigma,\Gamma,\sigma,q_0,F)$$ computes as follows. It accepts input $$w$$ if $$w$$ can be written as $$w=w_1w_2...w_m$$ (where $$w_i\in\Sigma_\epsilon$$), and sequences of states $$r_0,r_1,...,r_m$$(where $$w_i\in Q$$), and strings $$s_0,s_1,...,s_m$$ (其中$$s_i\in\Gamma^*$$) exists that satisfy the following three conditions. The string $$s_i$$ represent the sequence of stack contents that $$M$$ has on the accepting branch of the computation.

TODO..

##### 定理2.20（L(PDA) = L(CFG)）

A language is context free if and only if some pushdown automaton recognizes it.

> 证明方法：构造法，从CFG构造PDA，从PDA构造CFG

##### 推论2.32（regular languages $$\subset$$ context free languages）

Every regular language is context free

> 证明方法：每个regular language都有一个能识别它的FA，而FA是PDA结构简化版，即FAs$$\subseteq$$PDAs，因此 regular languages$$\subseteq$$L(PDA)=regular languages

##### 定理（$${CFLs}$$的封闭性）

对正则运算封闭，对交、补不封闭

