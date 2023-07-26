<div class="topSpace"></div>

Date Created: 29/12/2022 20:34:06
Tags: #Type/Proposition #Topic/Real_Analysis

Proved by: [[Characterizations of closure]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\tpl{X,d}$ be a metric space and fix $S\subseteq X$. Then, for all, $x\in X$, $x\in\bar{S}$ iff there exists a sequence $\tpl{x_n}$ in $S$ such that $x_n\to x$.

```

<i>Proof.</i> 
* ($\Rightarrow$): If $x\in\bar{S}$, then every neighborhood of $x$ intersects $S$. In particular, for all $n\in\N^+$, we have that $B_{1/n}\!\l(x\r)\cap S\neq\em$, so there exist $x_n\in S$ such that $d\l(x_n,x\r)<1/n$ for all $n\in\N^+$. Thus we obtain a sequence $\tpl{x_n}$ in $S$ such that $x_n\to p$, so we are done.

* ($\Leftarrow$): Let $\tpl{x_n}$ be a sequence in $S$ such that $x_n\to x$. Then, for any $\delta>0$, eventually we have $d\l(x_n,x\r)<\delta$. Thus $x_n\in B_\delta\!\l(x\r)$ eventually, and since $x_n\in S$, we have that $B_\delta\!\l(x\r)\cap S\neq\em$. Hence every neighborhood of $x$ intersects $S$, so $x\in\bar{S}$.<span style="float:right;">$\blacksquare$</span>
