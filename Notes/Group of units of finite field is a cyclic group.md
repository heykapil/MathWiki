---
mathLink: $\F^\times$ is a cyclic group
---

<div class="topSpace"></div>

Date Created: 07/05/2023 18:19:12
Tags: #Type/Proposition #Topic/Group_Theory #Topic/Ring_Theory

Proved by: [[At most one dividing subgroup implies cyclic]], [[Lagrange's Theorem]], [[Basic properties of order]], [[Polynomial has at most degree-many roots]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\F$ be a finite field. Then $\F^\times$ is cyclic.

```

<i>Proof.</i> Let $q\coloneqq\l|\F\r|$, so $\l|\F^\times\r|=q-1$. It suffices to show that every $p\divides\!\l(q-1\r)$ admits at most one subgroup $H$ of order $p$. Assume that such a subgroup $H\subgrpeq\F^\times$ exists. By Lagrange’s Theorem, every $h\in H$ has order dividing $p$, so $h^p=1$. Thus every $h\in H$ is a root of $x^p-1$. Conversely, since $x^p-1$ has at most $p$ roots and every $h\in H$ is a root, we see that $H$ consists of exactly the roots of $x^p-1$. In particular, this subgroup is unique.<span style="float:right;">$\blacksquare$</span>
