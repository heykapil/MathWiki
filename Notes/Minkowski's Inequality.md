---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 16/02/2023 10:42:25
Tags: #Type/Theorem #Topic/Real_Analysis/Later

Proved by: [[Holder's Inequality]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Theorem
title: Theorem (Minkowski’s Inequality).

Fix $n\in\N^+$ and take $\vec{x}\coloneqq\tpl{x_1,\dots,x_n}$ and $\vec{y}\coloneqq\tpl{y_1,\dots,y_n}$ in $\R^n$. For all $p\geq1$, we have
$$\begin{equation}
    \l(\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^p\r)^{1/p}\leq\l(\sum_{i=1}^{n}\l|x_i\r|^p\r)^{1/p}\!+\l(\sum_{i=1}^{n}\l|y_i\r|^p\r)^{1/p}=\|\vec{x}\|_p+\|\vec{y}\|_p.
\end{equation}$$

```

<i>Proof.</i> First, observe that the case for $p=1$ is trivial. For $p>1$, let $1<q<+\infty$ be its conjugate exponent. Observe that
$$\begin{equation}
    \sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^p=\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^{p-1}\l(\l|x_i\r|+\l|y_i\r|\r)=\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^{p-1}\l|x_i\r|+\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^{p-1}\l|y_i\r|.
\end{equation}$$
Applying Hölder’s Inequality, we see that
$$\begin{equation}
    \sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^{p-1}\l|x_i\r|\leq\l(\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^{\l(p-1\r)q}\r)^{1/q}\l(\sum_{i=1}^{n}\l|x_i\r|^p\r)^{1/p}.
\end{equation}$$
But $p$ and $q$ being conjugate exponents imply that $p=q\l(p-1\r)$, so we have
$$\begin{equation}
    \sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^{p-1}\l|x_i\r|\leq\l(\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^p\r)^{1/q}\l(\sum_{i=1}^{n}\l|x_i\r|^p\r)^{1/p}.
\end{equation}$$
Similarly, Hölder’s Inequality on the second factor gives
$$\begin{equation}
    \sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^{p-1}\l|y_i\r|\leq\l(\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^p\r)^{1/q}\l(\sum_{i=1}^{n}\l|y_i\r|^p\r)^{1/p},
\end{equation}$$
so we have
$$\begin{equation}
    \sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^p\leq\l(\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^p\r)^{1/q}\l[\l(\sum_{i=1}^{n}\l|x_i\r|^p\r)^{1/p}+\l(\sum_{i=1}^{n}\l|y_i\r|^p\r)^{1/p}\r].
\end{equation}$$
Diving, we obtain
$$\begin{equation}
    \l(\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^p\r)^{1/p}=\l(\sum_{i=1}^{n}\l(\l|x_i\r|+\l|y_i\r|\r)^p\r)^{1-\frac{1}{q}}\leq\l(\sum_{i=1}^{n}\l|x_i\r|^p\r)^{1/p}+\l(\sum_{i=1}^{n}\l|y_i\r|^p\r)^{1/p}.\qedin
\end{equation}$$
