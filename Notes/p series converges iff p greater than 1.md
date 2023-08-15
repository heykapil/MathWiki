---
mathLink: $p$-series converges $\Leftrightarrow$ $p>1$
---

<div class="topSpace"></div>

Date Created: 16/03/2023 10:15:25
Tags: #Type/Proposition #Topic/Real_Analysis

Proved by: [[Cauchy's Condensation Test]], [[Geometric Sequence]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Fix $p\in\R$. Then the infinite series $\sum_{k=1}^{\infty}1/k^p$ converges iff $p>1$.

```

<b>Remark.</b> In particular, with $p=1$, the <b>harmonic series</b> $\sum_{k=1}^{\infty}1/k$ diverges.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i> Clearly the series $\sum_{k=1}^{\infty}1/k^p$ diverges if $p\leq0$. Otherwise, if $p>0$, the sequence $\tpl{1/k^p}$ is non-increasing. By Cauchy Condensation, we consider the series
$$\begin{equation}
    \sum_{k=0}^{\infty}2^k\cdot\frac{1}{\l(2^k\r)^p}=\sum_{k=0}^{\infty}\frac{2^k}{2^{kp}}=\sum_{k=0}^{\infty}2^{\l(1-p\r)k}.
\end{equation}$$
This is a geometric series with common ratio $2^{\l(1-p\r)}$, so it converges iff $p>1$.<span style="float:right;">$\blacksquare$</span>
