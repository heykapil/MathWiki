---
mathLink: $\pi_1\!\l(X\r)=0$ $\Leftrightarrow$ all paths are homotopic
---

<div class="topSpace"></div>

Date Created: 17/05/2023 23:48:46
Tags: #Type/Proposition #Topic/Topology

Proved by: [[Basic properties of homotopies of paths]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X$ be a path-connected topological space and fix $x_0,x_1\in X$. Then $\pi_1\!\l(X\r)=0$ iff every pair of paths $\gamma_0,\gamma_1:\l[0,1\r]\to X$ from $x_0$ to $x_1$ are homotopic.

```

<i>Proof.</i> Let $\epsilon_0$ denote the constant path at $x_0$.
* ($\Rightarrow$). Since $X$ is path-connected, there exists a path $\sigma:\l[0,1\r]\to X$ from $x_0$ to $x_1$. Since $\gamma_1^-\ast\gamma_0$ is a loop at $x_0$ and $\pi_1\!\l(X\r)=0$, we see that $\gamma_1^-\ast\gamma_0\htopeq\epsilon_0$. Thus $\gamma_0\htopeq\gamma_1\ast\gamma_1^-\ast\gamma_0\htopeq\gamma_1\ast\epsilon_0\htopeq\gamma_1$, as desired.
* ($\Leftarrow$). Every loop $\gamma:\l[0,1\r]\to X$ at $x_0$ is by assumption homotopic to $\epsilon_0$, so $\pi_1\!\l(X\r)$ contains only one homotopy class $\l[\epsilon_0\r]$ and hence vanishes.<span style="float:right;">$\blacksquare$</span>
