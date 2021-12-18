# 3.1 Turing Machines

有一条无限长的tape，有一个可以读、写、左移、右移的tape head.

（你比...就在于你可以拿笔写下来）

##### 定义3.3（TM）

A ***Turing machine*** is a 7-tuple $$(Q,\Sigma,\Gamma,\sigma,q_0,q_{accept},q_{reject})$$, where $$Q$$, $$\Sigma$$, $$\Gamma$$ are all finite sets, and

1. $$Q$$ is the set of states,
2. $$\Sigma$$ is the input alphabet not containing the blank symbol $$\square$$,
3. $$\Gamma$$ is the tape alphabet, where $$\square\in\Gamma$$ and $$\Sigma\subseteq\Gamma$$,
4. $$\sigma:Q\times\Gamma\rightarrow Q\times \Gamma\times\{L,R\})$$ is the transition function
5. $$q_0\in Q$$ is the start state,
6. $$q_{accept}\in Q$$ is the accept state, and
7. $$q_{reject\in}Q$$ is the reject state, where $$q_{reject}\neq q_{accept}$$

##### 定义（TM's computation）

TM在任意时刻下的全部信息称为***configuration***，包含：the current state, the current tape contents, and the current head location. 特殊地：

- The ***start configuration*** is $$q_0w$$.
- In an ***accepting configuration***, the state of configuration is $$q_{accept}$$.
- In an ***rejecting configuration***, the state of configuration is $$q_{reject}$$.
- Accepting configurations and rejecting configurations are ***halting configurations***.

A Turing machine M ***accepts*** input $$w$$ if a sequence of configurations $$C_1,C_2,..., C_k$$ exists, where

1. $$C_1$$ is the start configuration of $$M$$ on input $$w$$
2. each $$C_i$$ yields $$C_{i+1}$$, and
3. $$C_k$$ is an accepting configuration

##### 定义3.5（Turing-recognizable）

Call a language ***Turing-recognizable*** if some TM accepts it.

> 当$$w\in M$$时，$$M$$在$$w$$上停机接受
>
> 当$$w\notin M$$时，$$M$$在$$w$$上停机拒绝或不停机

##### 定义3.6（Turing-decidable）

> 图灵机面对一个输入时，有accept, reject, looping三种可能的最终结果。如果一个TM对一个language种的输入总能回答accept or reject，那么称该TM ***decides***该language.

Call a language ***Turing-decidable*** or simply ***decidable*** if some TM decides it.

> 当$$w\in M$$时，$$M$$在$$w$$上停机接受
>
> 当$$w\notin M$$时，$$M$$在$$w$$上停机拒绝
