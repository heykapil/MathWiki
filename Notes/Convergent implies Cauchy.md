---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 25/11/2022 20:24:43
Tags: #Type/Proposition #Topic/Real_Analysis

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X$ be a metric space and consider a sequence $\tpl{x_n}$ in $X$. If $\tpl{x_n}$ converges, then it is Cauchy.

```

<i>Proof.</i> Suppose that $x_n\to l$ as $n\to\infty$ for some $l\in\R$, and let $\epsilon>0$. Then $\fa^\infty n\in\N:d\l(x_n,l\r)<\epsilon/2$, so
$$\begin{equation}
    d\l(x_n,x_m\r)\leq d\l(x_n,l\r)+d\l(x_m,l\r)<\epsilon/2+\epsilon/2=\epsilon
\end{equation}$$
for all eventually $m,n\in\N$.<span style="float:right;">$\blacksquare$</span>
