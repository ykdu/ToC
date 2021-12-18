# 1.3  Regular Expressions

##### 定义1.52（regular expression）

> regular expression可以理解成language之间的操作。
>
> 比如 $$(0\cup 1)$$\\$$s^*$$

Say that $$R$$ is a ***regular expression*** if $$R$$ is

1. $$a$$，for $$a\in\Sigma$$,
2. $$\sigma$$,
3. $$\emptyset$$,
4. $$(R_1\cup R_2)$$, where $$R_1$$ and $$R_2$$ are regular expressions,
5. $$(R_1\cdot R_2)$$, where $$R_1$$ and $$R_2$$ are regular expressions, or
6. $$(R_1^*)$$, where $$R_1$$ is regular expressions,

> 虽然只有三个operation，但很多其他operations可以构造出来，比如$$R^+$$，补、交



##### 定理（L(RE) = L(FA））

A language is regular if and only if some regular expression describes it

> 证明方法：引入GNFA来证明充分性，构造法证明必要性；
>
> FA和RE有相同的表达能力

