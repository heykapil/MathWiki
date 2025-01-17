---
mathLink-blocks:
    torsion-free-iff-free: Torsion-free $\Leftrightarrow$ free (PID)
---

<div class="topSpace"></div>

Date Created: 23/07/2023 20:04:42
References: #Ref/Alu09
Tags: #Type/Proposition #Topic/Rings_and_Modules

Proved by: [[Freedom Theorem for Modules over PID]], [[Basic properties of rank]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition (Characterizations of PIDs).

Let $R$ be an integral domain. Then $R$ is a PID iff any of the following hold.
* For every finitely-generated $R$-module $M$ and every exact sequence $R^n\overset{\pi}{\longrightarrow}M\longrightarrow0$, there is a free $R$-module $R^m$ for some $m\leq n$ and a homomorphism $\phi:R^m\to R^n$ making $0\longrightarrow R^m\overset{\phi}{\longrightarrow}R^n\overset{\pi}{\longrightarrow}M\longrightarrow0$ exact.
* Every finitely-generated $R$-module is torsion-free iff it is free.

```
^torsion-free-iff-free

<i>Proof.</i> Assume that $R$ is a PID. The two statements are then corollaries of the Freedom Theorem for PIDs. Indeed, let $\pi:R^n\onto M$ be a surjection.
* The kernel of $\pi$ is a submodule of the free module $R^n$, which is itself free, so there is an isomorphism $\phi:R^m\to\ker\pi$ for some $m\leq n$.
* Furthermore, there is a basis $\tpl{x_i}_{i=1}^n$ of $R^n$ and non-zero elements $\tpl{a_j}_{j=1}^m$ of $R$ with $a_1\divides\cdots\divides a_m$ such that $\tpl{a_jx_j}_{j=1}^m$ is a basis for $\ker\pi$. Consider the surjective $R$-module homomorphism
$$\begin{equation}
    R^n\to R^{n-m}\oplus\bigoplus_{j=1}^{m}R/\!\gen{a_j}\ \ \ \ \ \ \ \ \textrm{mapping}\ \ \ \ \ \ \ \ \sum_{i=1}^nr_ix_i\mapsto\tpl{r_{m+1},\dots,r_n,r_1+\gen{a_1},\dots,r_m+\gen{a_m}}.
\end{equation}$$
Its kernel is $\ker\pi$, whence $M\iso R^n/\ker\pi\iso R^{n-m}\oplus\bigoplus_{j=1}^mR/\!\gen{a_j}$. Thus $\Tor M\iso\bigoplus_{j=1}^mR/\!\gen{a_j}$, so if $M$ is torsion-free, then $M\iso R^{n-m}$ is free. Conversely, every free-module is torsion-free.

Conversely, let $\mf{a}\nsubgrpeq R$ be an ideal and consider the homomorphism $\pi:R^1\to R/\mf{a}$. It suffices to show that $\mf{a}$ is free, whence $\mf{a}\iso R^0$ is trivial or $\mf{a}\iso R^1$ is generated by a single element.
* An exact sequence $0\to R^m\to R^1\to R/\mf{a}\to0$ shows that $\mf{a}=\ker\pi=\im\phi$ is isomorphic to $R^m$, so it is free.
* Since $R$ is an integral domain, we see that $\mf{a}$ is torsion-free as an $R$-submodule of $R$, so $\mf{a}$ is free.<span style="float:right;">$\blacksquare$</span>
