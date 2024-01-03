---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 21/03/2023 10:19:54
References: #Ref/Rud76
Tags: #Type/Proposition #Topic/Real_Analysis

Proved by: [[Abel's Summation Formula]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition (Dirichlet’s Test).

Let $\tpl{a_k}$ and $\tpl{b_k}$ be sequences in $\R$. If $\tpl{a_k}$ is non-increasing, $a_k\to0$, and the partial sums of $\tpl{b_k}$ are bounded, then $\sum_{k=1}^{\infty}a_kb_k$ converges.

```

<b>Remark.</b> In particular, setting $b_k\coloneqq\l(-1\r)^k$ yields the <b>alternating series test</b>.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i> Let $s_n$ be the sequence of partial sums of $b_k$. Since $s_n$ is bounded, there exists some $B\in\R$ such that $\l|s_n\r|\leq B$ for all $n\in\N$. By Abel’s formula, we see that
$$\begin{equation}
    \l|\sum_{k=n+1}^{m}a_kb_k\r|=\l|\l(a_ms_m-a_{n+1}s_n\r)+\sum_{k=n+1}^{m-1}\l(a_k-a_{k+1}\r)s_k\r|\leq\l|a_ms_m\r|+\l|a_{n+1}s_n\r|+\sum_{k=n+1}^{m-1}\l|a_k-a_{k+1}\r|s_k\leq B\l[a_m+a_{n+1}+\sum_{k=n+1}^{m-1}\l(a_k-a_{k+1}\r)\r]
\end{equation}$$
for all $m>n$. This sum telescopes to
$$\begin{equation}
    \l|\sum_{k=n+1}^{m}a_kb_k\r|\leq B\l(a_m+a_{n+1}+a_{n+1}-a_m\r)=2Ba_{n+1}.
\end{equation}$$
But $a_k\to0$, so this can be bounded by an arbitrary $\epsilon>0$, from which the result follows by the Cauchy Criterion.<span style="float:right;">$\blacksquare$</span>
