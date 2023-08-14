---
mathLink: $\sqrt[n]{a}\to1$
---

<div class="topSpace"></div>

Date Created: 04/10/2022 15:11:41
Tags: #Type/Proposition #Topic/Real_Analysis

Proved by: [[Bernoulli's Inequality]], [[Limit of 1 over linear]], [[Squeezed Distance Lemma]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

For all $a\in\R^+$, we have $\lim\limits_{n\to\infty}\sqrt[n]{a}=1$.

```

<i>Proof.</i> If $a=1$, then $\sqrt[n]{a}=1$ is the constant sequence, which converges to $1$. We consider the cases for when $a<1$ and $a>1$.
* ($a>1$): We claim that $\sqrt[n]{a}>1$; if $\sqrt[n]{a}\leq1$, then $a\leq 1^n=1$, a contradiction. Set $d_n\coloneqq\sqrt[n]{a}-1>0$. It suffices to show that $d_n\to0$ as $n\to\infty$, for then $\sqrt[n]{a}\to1$ as $n\to\infty$. Observe that $\sqrt[n]{a}=1+d_n$, so, by Bernoulli' Identity, $a=\l(1+d_n\r)^n\geq1+nd_n$. Thus
$$\begin{equation}
    d\l(d_n,0\r)=\l|d_n\r|=d_n\leq\frac{a-1}{n}=\l(a-1\r)\cdot\frac{1}{n},
\end{equation}$$
and since $1/n\to0$ as $n\to\infty$, the result follows.

* ($a<1$): We claim $\sqrt[n]{a}<1$; if $\sqrt[n]{a}\geq1$, then $a\geq1^n=1$, a contradiction. Hence $1/\sqrt[n]{a}>1$, so set $d_n\coloneqq\frac{1}{\sqrt[n]{a}}-1>0$. Similarly, it suffices to show that $d_n\to0$ as $n\to\infty$. Observe that $\sqrt[n]{a}=\frac{1}{1+d_n}$, so, by Bernoulli' Identity,
$$\begin{equation}
    a=\frac{1}{\l(1+d_n\r)^n}\leq\frac{1}{1+nd_n}.
\end{equation}$$
But then $1+nd_n\leq1/a$, so
$$\begin{equation}
    d\l(d_n,0\r)=\l|d_n\r|=d_n\leq\l(\frac{1}{a}-1\r)\cdot\frac{1}{n}.
\end{equation}$$
Since $1/n\to0$ as $n\to\infty$, the result follows.<span style="float:right;">$\blacksquare$</span>
