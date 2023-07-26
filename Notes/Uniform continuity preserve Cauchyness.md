<div class="topSpace"></div>

Date Created: 25/11/2022 19:43:43
Tags: #Type/Proposition #Topic/Real_Analysis

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $f:X\to Y$ be a uniformly continuous function between metric spaces. If a sequence $\tpl{x_n}$ in $X$ is Cauchy, then so is the sequence $\tpl{f\l(x_n\r)}$ in $Y$.

```

<i>Proof.</i> Let $\tpl{x_n}$ be a Cauchy sequence in $X$ and take $\epsilon>0$. Then, since $f$ is uniformly continuous,
$$\begin{equation}
    \ex\delta>0,\fa S\subseteq X:\diam S\leq\delta\Rightarrow\diam\im_f\l(S\r)\leq\epsilon.
\end{equation}$$
But $\tpl{x_n}$ is Cauchy, so $\diam\l\{x_N,x_{N+1},\dots\r\}\leq\delta$ for all eventually $N\in\N$ and hence $\diam\im_f\l\{x_N,x_{N+1},\dots\r\}\leq\epsilon$ for all eventually $N\in\N$. Observe then that
$$\begin{equation}
    \fa^\infty N\in\N:\diam\l\{f\l(x_N\r),f\l(x_{N+1}\r),\dots\r\}\leq\epsilon,
\end{equation}$$
so $\tpl{f\l(x_n\r)}$ is Cauchy.<span style="float:right;">$\blacksquare$</span>
