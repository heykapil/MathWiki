---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 07/02/2022 14:15:40
Tags: #Type/Proposition #Topic/Topology/Later

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\tpl{\R^2,\mc{T}}$ be the topological space where $\mc{T}\coloneqq\mc{T}\l(\mc{B}\r)$ is the lexicographical order topology on $\R^2$. Then sets of the form $U\coloneqq\l(m,n\r)\times\R$ where $m,n\in\R$ are open but not basis elements in $\mc{B}$.

```

<i>Proof.</i> To show that $U\in\mc{T}\l(\mc{B}\r)$, it suffices to find some subset $\mc{A}\subseteq\mc{B}$ with $U=\bigcup\mc{A}$. Indeed, let
$$\begin{equation}
    \mc{A}\coloneqq\l\{A\in\pow\l(\R^2\r)\st\ex a,b,c,d\in\R:m<a\leq c<n\land A=\l(\tpl{a,b},\tpl{c,d}\r)\r\}
\end{equation}$$
and set $V\coloneqq\bigcup\mc{A}$; we wish to show that $U=V$.
* ($U\subseteq V$). Take $\tpl{x,y}\in U$, so $m<x<n$. Observe that
$$\begin{equation}
    \tpl{x,y}\in\l(\tpl{x,y-1},\tpl{x,y+1}\r)\in\mc{A},
\end{equation}$$
so $\tpl{x,y}\in\bigcup\mc{A}=V$.

* ($V\subseteq U$). Take $v\in V=\bigcup\mc{A}$, so $\ex A\in\mc{A}:v\in A$. In other words, there exist $a,b,c,d\in\R$ with $m<a\leq c< n$ such that $v\in\l(\tpl{a,b},\tpl{c,d}\r)$. Let $v\coloneqq\tpl{v_1,v_2}$, so, in particular, we have $a\leq v_1\leq c$ and thus $m<v_1<n$. It follows that $v_1\in\l(m,n\r)$ and hence $v\in U$.

It remains to show that $U$ is not a basis element in $\mc{B}$. Suppose, for sake of contradiction, that there exist $\alpha\coloneqq\tpl{a,b}\in\R^2$ and $\beta\in\R^2$ such that $U=\l(\alpha,\beta\r)$.
* If $a\geq n$, then any element in $U$, say $p\coloneqq\tpl{\frac{m+n}{2},0}$, does not lie in $\l(\alpha,\beta\r)$.
* If $m<a<n$, then $q\coloneqq\tpl{a,b-1}\in U$ but does not lie in $\l(\alpha,\beta\r)$.
* If $a\leq m$, then $r\coloneqq\tpl{a,b+1}\in U$ but does not lie in $\l(\alpha,\beta\r)$.

In each ease, we see that $U\neq\l(\alpha,\beta\r)$ and is hence not a basis element in $\mc{B}$.<span style="float:right;">$\blacksquare$</span>
