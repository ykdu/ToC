# 7.3 The Class NP

##### 定义7.18（verifier）

A ***verifier*** for a language $$A$$ is an algorithm $$V$$, where

​				$$A=\{w|V$$ accepts $$<w,c>$$ for some string $$c\}$$.

We measure the time of a verifier only in terms of the length of $$w$$, so a ***polynomial time verifier*** runs in polynomial time in the length of $$w$$.

$$c$$ is called a ***certificate***.

##### 定义7.19（NP）

$$NP$$ is the class of languages that have polynomal time verifiers.

##### 定理7.20（NP=L(NTM)）

A language is in NP iff it is decided by some nondeterministic polynomial time Turing machine.

##### 定义7.21（NTIME language集合）

NTIME(t(n))$$=\{L|L$$ is a language decided by an O(t(n)) time nondeterministic TM$$\}$$

##### 推论7.22（）

$$NP=\bigcup\limits_{k}$$NTIME$$(n^k)$$.

##### 定理7.24（NP例子——CLIQUE）

$$CLIQUE=\{<G,k>|G$$ is an undirected graph with a $k$-cliqui$$\}$$.

$$CLIQUE$$ is in NP.

#### P=NP ?

目前已知的NP的最小上界是EXP。是否还有更小的上界（甚至是否P是上界），还不可知。

$$NP\subseteq$$EXPTIME$$=\bigcup\limits_{k}$$ TIME $$(2^{n^k})$$,

