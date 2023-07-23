<div class="topSpace"></div>

Date Created: 22/01/2022 09:43:31
Tags: #Type/Proposition #Topic/Set_Theory/Later

Proved by: [[Inverse of a relation is a relation]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $R$ be a binary relation. Then $\l(R^{-1}\r)^{-1}=R$.

```

<i>Proof.</i> By definition, we have $R^{-1}=\l\{\tpl{y,x}\st xRy\r\}$. Taking the inverse again, we have

$\begin{alignat}{2}
    \l(R^{-1}\r)^{-1}&=\l\{\tpl{x,y}\st yR^{-1}x\r\}\\
    &=\l\{\tpl{x,y}\st xRy\r\}\\
    &=R.\qedin
\end{alignat}$
