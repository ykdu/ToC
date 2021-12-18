# 5.2 A Simple Undecidable Problem

##### 定理5.15（PCP）

***Post Correspondence Problem***：Begin with a collection of dominos. The task is to make a list of given deminos***(repetitions permitted)*** so that the string we get by reading off the symbols on the top is the same as the string of symbols on the bottom. This list is called a ***match***.

$$PCP=\{<P>|P$$ is an instance of the PCP with a match$$\}$$

$$PCP$$ is undecidable.

> PCP是Turing-recognizable的，只要从1开始枚举所有不同长度的排列，如果存在解则一定能accept
>
> 证明方法：computation histories

TODO

