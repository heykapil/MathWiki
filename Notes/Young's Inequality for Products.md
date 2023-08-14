---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 14/02/2023 11:14:24
Tags: #Type/Proposition #Topic/Real_Analysis

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition (Young’s Inequality for Products).

Let $a,b\in\R_0^+$ and let $1<p,q<+\infty$ be conjugate exponents. Then $ab\leq\frac{a^p}{a}+\frac{b^q}{q}$.

```

<i>Proof.</i> Recall that a twice differentiable function $f:\R\to\R$ with $f''\l(x\r)\geq0$ for all $x$ is convex; that is
$$\begin{equation}
    f\l(\alpha t+\beta\l(1-t\r)\r)\leq tf\l(\alpha\r)+\l(1-t\r)f\l(\beta\r)
\end{equation}$$
for every $\alpha,\beta\in\R$ and $t\in\l[0,1\r]$. Noting that $e^x$ is convex, we take $\alpha\coloneqq p\ln a$, $\beta\coloneqq q\ln b$, and $t\coloneqq 1/p$ to give
$$\begin{equation}
    e^{\ln a+\ln b}\leq\frac{e^{p\ln a}}{p}+\frac{e^{q\ln b}}{q}.
\end{equation}$$
Simplifying gives the desired result.<span style="float:right;">$\blacksquare$</span>
