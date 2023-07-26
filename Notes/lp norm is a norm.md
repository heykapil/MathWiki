---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 16/02/2023 11:00:59
Tags: #Type/Proposition #Topic/Real_Analysis/Later

Proved by: [[Minkowski's Inequality]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Fix $p\in\l[1,+\infty\r)$ and consider the function $\|\slot\|:\ell^p\to\R$ defined by
$$\begin{equation}
    \|\vec{x}\|_p\coloneqq\l(\sum_{i=1}^{n}\l|x_i\r|^p\r)^{1/p}
\end{equation}$$
for all $\vec{x}\coloneqq\tpl{x_1,\dots,x_n}\in\R^n$.

```

<i>Proof.</i> Positive-definiteness and absolute homogeneity are clear. For the triangle inequality, take $\vec{x},\vec{y}\in\R^n$. Note that $\l|x_i+y_i\r|\leq\l|x_i\r|+\l|y_i\r|$ for all $1\leq i\leq n$, and since the function $z\mapsto z^p$ is increasing for all $z>0$, we see that $\l|x_i+y_i\r|^p\leq\l(\l|x_i\r|+\l|y_i\r|\r)^p$. Observe then that
$$\begin{equation}
    \|\vec{x}+\vec{y}\|_p=\l(\sum_{i=1}^{n}\l|x_i+y_i\r|^p\r)^{1/p}\leq\l(\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^p\r)^{1/p}\leq\l(\sum_{i=1}^{n}\l|x_n\r|^p\r)^{1/p}\!+\l(\sum_{i=1}^{n}\l|y_n\r|^p\r)^{1/p}=\|\vec{x}\|_p+\|\vec{y}\|_p
\end{equation}$$
where the second inequality follows from the Minkowski’s Inequality.<span style="float:right;">$\blacksquare$</span>
