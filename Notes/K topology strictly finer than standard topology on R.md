---
mathLink: $\KtopR$ strictly finer than $\sttopR$
---

<div class="topSpace"></div>

Date Created: 05/02/2022 11:07:34
Tags: #Type/Proposition #Topic/Topology/Later

Proved by: [[Q is dense in R]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\R$ be the set of real numbers. Then the $K$ topology $\KtopR$ is strictly finer than the standard topology $\sttopR$ on $\R$.

```

<i>Proof.</i> Take $\l(a,b\r)\in\mc{B}_\textrm{st}$ and $x\in\l(a,b\r)$. The same interval $\l(a,b\r)\in\mc{B}_K$ contains $x$ and is a subset of itself, so $\sttopR\subseteq\KtopR$. The converse does not hold, for let $\l(-1,1\r)\comp K\in\mc{B}_K$ and choose $x=0$. Any $\l(e,f\r)\in\mc{B}_\textrm{st}$ containing $x$ necessarily contains some $q=1/n$ for large enough $n$, so $\l(e,f\r)\not\subseteq\l(-1,1\r)\comp K$. Thus $\sttopR\subset\KtopR$.<span style="float:right;">$\blacksquare$</span>
