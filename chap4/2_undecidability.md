# 4.2 Undecidability

One of the most philosophically important theorems os the theory of computation: There is a specific problem that is algorithmically unsolvable.

##### 定义（Universal Turing Machine）

$$A_{TM}=\{<M,w>|M$$ is a TM and $$M$$ accepts $$w\}$$

> 使用M的alphabet对M进行编码

##### 定理（an undecidable language，（最基础的“算法不可实现问题“））

$$A_{TM}$$ is undecidable

> 证明方法：对角化方法 + countable概念 + 构造

有没有Turing-recognizable之外的language呢？

> 有。因为：
>
> All TMs is countable，即Turing-recognizable languages is countable
>
> All languages is uncountable
>
> 所以必然有

##### 定理4.22

A Language $$L$$ is decidable iff $$L$$ and $$\overline{L}$$ are both Turing-recognizable.

> 证明方法：构造法

##### 推论4.23（an unrecognizable language）

$$\overline{A_{TM}}$$ is not Turing-recognizable

> 反证，如若是Turing-recognizable，则$$A_{TM}$$是decidable

