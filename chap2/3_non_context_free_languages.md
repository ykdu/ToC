# 2.3 Non-Context-Free Languages

Q：如何证明一个language***不是***context-free language？

A：证明它违背了***pumping lemma for context-free languages***是一个常用方法。（反证：假设是cfl，则寻找一个p，使得不满足pumping lemma）

##### 定理（Pumping lemma for context-free languages）

> 一个context-free string必然可拆解成一个带两环的形式，将两环进行任意次循环后的string都依然是context-free string。

