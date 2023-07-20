<div class="topSpace"></div>

Date Created: 23/04/2022 12:48:57
Tags: #Type/Proposition #Later/Module_Theory

Proved by: [[Basis Extension Theorem]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $K$ be a field and let $V$ be a finite-dimensional vector space over $K$. If $W$ is a subspace of $V$, then $W$ is finite-dimensional and $\dim W\leq\dim V$. Furthermore, $\dim W<\dim V$ iff $W\subset V$.

```

<i>Proof.</i> Let $\mc{B}_W$ be a basis for $W$; since it is a linearly independent subset of $V$, we may extend it to a basis $\mc{B}_V$ of $V$ with $\mc{B}_W\subseteq\mc{B}_V$. Since $\l|\mc{B}_V\r|<\infty$, we see that $\l|\mc{B}_W\r|\leq\l|\mc{B}_V\r|<\infty$ too and hence $W$ is finite-dimensional with $\dim W\leq\dim V$.
* ($\Rightarrow$): If $W=V$, then $\dim W=\dim V$ trivially. Thus, by contradiction, we have $W\subset V$.

* ($\Leftarrow$): Since $W\subset V$, there exists $v\in V$ with $v\not\in W=\span\mc{B}_W$. Thus $\mc{B}_W\cup\l\{v\r\}$ is a linearly independent subset of $V$, and since $\span\mc{B}_V=V$, we see that $\l|\mc{B}_W\cup\l\{v\r\}\r|\leq\l|\mc{B}_V\r|$; the result follows since $\mc{B}_W\cap\l\{v\r\}=\em$, so $\l|\mc{B}_W\cup\l\{v\r\}\r|=\dim W+1\leq\dim V$.<span style="float:right;">$\blacksquare$</span>
