# 1.4 Nonregular Languages

Q：如何证明一个language***不是***regular language？

A：证明它违背了pumping lemma是一个常用方法。（反证：假设是RL，则寻找一个p，使得不满足pumping lemma）

##### 定理（Pumping lemma）

> 一个regular string必然可拆解成一个带环的形式，将环进行任意次循环后的string都依然是regular string。

