<div class="topSpace"></div>

Date Created: 23/10/2022 20:05:35
Tags: #Type/Theorem #Topic/Real_Analysis

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Theorem
title: Theorem (Monotone Subsequence Theorem).

Let $\tpl{x_n}_{n\in\N}$ be a sequence in $\R$. Then there exists a monotone subsequence $\tpl{x_{n_k}}_{k\in\N}$ of $\tpl{x_n}$.

```

<i>Proof.</i> Call a term $x_m$ in $\tpl{x_n}$ a <b>peak</b> if $x_m\geq x_n$ for all $n\geq m$.
* If $\tpl{x_n}$ contains infinitely-many peaks, say $\tpl{x_{m_k}}_{k\in\N}$, then
$$\begin{equation}
    x_{m_1}\geq x_{m_2}\geq\cdots\geq x_{m_{k}}\geq\cdots.
\end{equation}$$
Thus $\tpl{x_{m_k}}$ is a monotonically decreasing subsequence of $\tpl{x_n}$.

* If $\tpl{x_n}$ contains finitely-many peaks (perhaps none), let $s_1\coloneqq m_k+1$ be the first index after the last peak. Thus $x_{s_1}$ is not a peak, so there exists some $s_2>s_1$ such tat $x_{s_1}<x_{s_2}$. Similarly, there exists some $s_3>s_2$ such that $x_{s_2}<x_{s_3}$, so we continue this way to obtain a monotonically increasing subsequence $\tpl{x_{s_k}}$ of $\tpl{x_n}$.<span style="float:right;">$\blacksquare$</span>
