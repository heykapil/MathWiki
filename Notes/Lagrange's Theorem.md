---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 13/10/2022 12:03:14
Tags: #Type/Theorem #Topic/Group_Theory

Proved by: <i>Not Applicable</i>
References: [[Basic properties of order]]
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: [[Orbit-Stabilizer Theorem]]

``` ad-Theorem
title: Theorem (Lagrange’s Theorem).

Let $H\subseteq G$ be a subgroup of a finite group $G$. Then $\l[G:H\r]\cdot\ord{H}=\ord{G}$.

```

<b>Remark.</b> Thus the order of every subgroup $H\subseteq G$ divides the order of $G$. Some immediate corollaries:
* For all $g\in G$, $\ord{g}$ divides $\ord{G}$. Indeed, since $\ord{g}=\ord{\gen{g}}$ and $\ord{\gen{g}}$ divides $\ord{G}$, we are done.

* If $p\coloneqq\l|G\r|$ is prime, then $G=\gen{x}$ for each non-trivial $x\in G$. Indeed, since $\ord{x}$ divides $p$ and $p$ is prime, either $\ord{x}=1$ or $\ord{x}=p$. But $x$ is non-trivial, so $\ord{x}=p$ and hence $\gen{x}=G$.
* If $K\subseteq H\subseteq G$ are all subgroups, then $\l[G:K\r]=\l[G:H\r]\l[H:K\r]$. Indeed, 
$$\begin{equation}
    \l[G:K\r]=\frac{\ord{G}}{\ord{K}}=\frac{\ord{G}}{\ord{H}}\frac{\ord{H}}{\ord{K}}=\l[G:H\r]\cdot\l[H:K\r].\exqedin
\end{equation}$$

---

<i>Proof.</i> Let $n\coloneqq\l[G:H\r]$ be the number of left-cosets of $H$ in $G$. Since the left-cosets of $H$ in $G$ partition $G$, we see that $G=\coprod_{i=1}^ng_iH$. But every coset of $H$ has the same cardinality as $H$, so $\l|g_iH\r|=\ord{H}$ for all $i\in\l\{1,\dots,n\r\}$. Thus $\ord{G}=n\ord{H}=\l[G:H\r]\cdot\ord{H}$.<span style="float:right;">$\blacksquare$</span>
