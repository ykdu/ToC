# 4.1 Decidable Languages

##### 记号（$$<>$$）

$$<A>$$代表A编码成的string

> TM的输入必须是string，比如多项式、图、TM等对象都可以编码



##### 定理（判定行、空性、等价性）

Let

$$A_{FA}=\{<B,w>|B$$ is a FA that accepts input string $$w\}$$

$$E_{FA}=\{<B>|B$$ is a FA and $$L(B)=\emptyset\}$$

$$EQ_{FA}=\{<A,B>|A$$ and $$B$$ are FAs and $$L(A)=L(B)\}$$

则

$$A_{FA}$$ is a decidable language

$$E_{FA}$$ is a decidable language

$$EQ_{FA}$$ is a decidable language

$$A_{CFG}$$ is a decidable language

Every context-free language is decidable

$$E_{CFG}$$ is a decidable language
