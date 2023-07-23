<div class="topSpace"></div>

Date Created: 21/01/2022 11:24:19
Tags: #Type/Proposition #Topic/Set_Theory/Later

Proved by: [[Binary relation iff subset of Cartesian product]], [[Axiom Schema of Specification]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $R$ be a binary relation. Then there exists a unique binary relation $R^{-1}$ whose elements are exactly the pairs $\tpl{y,x}$ where $\tpl{x,y}\in R$.

```

<i>Proof.</i> We shall first construct the set $R^{-1}$ with the prescribed properties and then prove that this set is indeed a binary relation.
* Formally, the existence of the set $R^{-1}$ is justified with the following statement:
$$\begin{equation}
    \fa R\l[R\textrm{ is a binary relation }\Rightarrow\ex!z\l(w\in z\Leftrightarrow\ex x\ex y\l(xRy\land w=\tpl{y,x}\r)\r)\r].
\end{equation}$$
Indeed, if $\ex x\ex y\l(xRy\land w=\tpl{y,x}\r)$, we have that $\tpl{x,y}\in\dom R\times\ran R$ and thus $w=\tpl{y,x}\in\ran R\times\dom R$. $\axispec$ then justifies the construction
$$\begin{equation}
    R^{-1}\coloneqq\l\{\tpl{y,x}\st xRy\r\}\coloneqq\l\{w\in\ran R\times\dom R\st\ex x\ex y\l(xRy\land w=\tpl{y,x}\r)\r\}.
\end{equation}$$
* Observe that $R^{-1}\subseteq\ran R\times\dom R$, so $R^{-1}$ is a binary relation.<span style="float:right;">$\blacksquare$</span>
