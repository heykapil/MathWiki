---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 27/05/2023 16:35:51
Tags: #Type/Proposition #Topic/Topology

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X$ be a path-connected and locally path-connected space. For an action $\phi:G\act X$, the quotient $p:X\to X/G$ is a covering map iff every $x\in X$ admits a neighborhood $U\ni x$ such that $gU\cap U\neq\em$ forces $g=\id$ for all $g\in G$.

```

<i>Proof.</i> If $p:X\to X/G$ is a covering map, then for every $x\in X$, the class $p\l(x\r)$ admits an evenly-covered neighborhood that lifts to a sheet $x\in U\subseteq X$. For any $g\in G$, if $gU\cap U\neq\em$, then there exist $x_1,x_2\in U$ such that $x_2=g\cdot x_1$. Observe then that $p\l(x_2\r)=p\l(g\cdot x_1\r)=p\l(x_1\r)$, so the local section of $p$ gives us $x_1=x_2$. Thus $g$ fixes a point, so $g=\id$ as desired.

Conversely, let $p\l(x\r)\in X/G$ and choose a neighborhood $U\ni x$ such that $gU\cap U\neq\em$ implies $g=\id$. We claim that $p\l(U\r)$ is an evenly-covered neighborhood of $p\l(x\r)$.
* Since $p^{-1}\!\l(p\l(U\r)\r)=\coprod_{g\in G}gU$ is open, we see that $p\l(U\r)$ is open too. Furthermore, $gU\cap hU=\em$ unless $g=h$, so the union is disjoint. Lastly, $\l.p\r|_{gU}:gU\to p\l(U\r)$ is a bijection since if $p\l(gx_1\r)=p\l(gx_2\r)$ for some $x_1,x_2\in U$, then $gx_1=hgx_2$ for some $h\in G$. Thus $h=e$, lest $h\l(gU\r)\cap\l(gU\r)\neq\em$, so $gx_1=gx_2$.<span style="float:right;">$\blacksquare$</span>