# 1.2 Nondeterminism

##### 定义1.5（NFA）

A ***nondeterministic finite autamation*** is a 5-tuple $$(Q,\Sigma,\sigma,q_0,F)$$, where

1. $$Q$$ is a finite set called the ***states***,
2. $$\Sigma$$ is a finite set called the ***alphabet***,
3. $$\sigma:Q\times\Sigma_\epsilon\rightarrow P(Q)$$ is the ***transition function***,
4. $$q_0\in Q$$ is the ***start state***,
5. $$F \subseteq Q$$ is the ***set of accept states***

>  $$P(Q)$$ 是Q的所有子集组成的集合
>
>  $$\Sigma_\epsilon = \Sigma \cup\{\epsilon\}$$

#### NFA特点

任意时刻，状态机可以同时处于多个可能状态，最终只要有一个状态被接受即为被接受。

NFA构造简单，分析复杂；DFA构造复杂，分析简单。

NFA存在可以产生备份，备份也会消失，这是物理不可实现的，因为不能随意产生消失。可以是软件，线程代表备份来产生、消失。DFA是物理可实现的。

##### 定义（equivalent）

Two machines are ***equivalent*** if they recognize the same language.

##### 定理（equivalence of DFAs and NFAs）

每台NFA都有equivalent DFA.

> 证明方法：构造法，给出了NFA和DFA之间相互构造的流程

##### 推论（regular language = L(NFA) = L(DFA)）

A language is regular if and only if some nondeterministic finite automaton recognizes it.

