---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 21/03/2023 11:06:31
Tags: #Proposition #Topics/Analysis

Proved by: _Not Applicable_
References: _Not Applicable_
Justifications: _Not Applicable_

Specializations: _Not Applicable_
Generalizations: _Not Applicable_

``` ad-Proposition
title: Proposition.

_Let $\tpl{a_k}$ be a sequence in $\R$ such that_ $S\coloneqq\sum_{k=0}^{\infty}a_k$ _converges absolutely. Then every rearrangement thereof converges to $S$._

```

_Proof_. The convergence of $\sum_{k=0}^{\infty}a_k$ shows that for every $\epsilon>0$, there exists some $N_1\in\N$ such that for all $n\geq N_1$, $\l|s_n-S\r|<\epsilon/2$. Furthermore, since $\sum_{k=0}^{\infty}\l|a_k\r|$ converges, there exists some $N_2\in\N$ such that $\sum_{k=N_2+1}^{q}\l|a_k\r|<\epsilon/2$ for all $q>M$. Set $N\coloneqq\max\l\{N_1,N_2\r\}$.

Consider a rearrangement $\sum_{k=0}^{\infty}b_k$ of $\sum_{k=0}^{\infty}a_k$, whose partials sums are, say $\tpl{t_n}$, and let $M\in\N$ be large enough so that $a_1,\dots,a_N$ are all terms in $t_M$. Thus, if $m\geq M$ and $n\geq N$, then $t_m-s_n$ is a finite sum of terms in $\tpl{a_k}$ with $k>N$. Thus, for some $q>N$, we have
$$\begin{equation}
    \l|t_m-s_n\r|\leq\sum_{k=N+1}^{q}\l|a_k\r|<\epsilon/2.
\end{equation}$$
Combining with our result above, we see that
$$\begin{equation}
    \l|t_m-S\r|\leq\l|s_n-S\r|+\l|t_m-s_n\r|<\epsilon
\end{equation}$$
for all $m\geq M$.<span style="float:right;">$\blacksquare$</span>