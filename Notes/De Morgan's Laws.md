---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 18/01/2022 16:48:35
Tags: #Type/Theorem #Topic/Set_Theory

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Theorem
title: Theorem (De Morgan’s Laws).

Let $V$ be a set and let $\l\{U_i\r\}_{i\in I}$ be a non-empty indexed family of sets. Then
$$\begin{equation}
    V\comp\bigcup_{i\in I}U_i=\bigcap_{i\in I}V\comp U_i\ \ \ \ \ \ \ \ \mathit{and}\ \ \ \ \ \ \ \ V\comp\bigcap_{i\in I}U_i=\bigcup_{i\in I}V\comp U_i.
\end{equation}$$

```

<i>Proof.</i> We shall prove the first statement, then use it to prove the second.
* Take $x\in V\comp\bigcup_{i\in I}U_i$. The first result follows from the following chain of equivalences:
$$\begin{equation}
    \begin{alignedat}{2}
        x\in V\comp\bigcup_{i\in I}U_i&\Leftrightarrow x\in V\land x\not\in\bigcup_{i\in I}U_i && \textrm{Definition of relative complement} \\
        &\Leftrightarrow x\in V\land\lnot\l(\ex i\in I:x\in U_i\r) && \textrm{Definition of union} \\
        &\Leftrightarrow x\in V\land\l(\fa i\in I:x\not\in U_i\r) && \textrm{Negation of quantifier} \\
        &\Leftrightarrow\fa i\in I:\l(x\in V\land x\not\in U_i\r) && i\textrm{ is not free in }x\in V \\
        &\Leftrightarrow\fa i\in I:x\in V\comp U_i && \textrm{Definition of relative complement} \\
        &\Leftrightarrow x\in\bigcap_{i\in I}V\comp U_i. && \l|I\r|\neq\em\textrm{; definition of intersection}
    \end{alignedat}
\end{equation}$$
The last equivalence requires that $\l|I\r|\neq\em$, which ensures that the intersection is defined.

* Consider the non-empty indexed family $\l\{U'_i\r\}_{i\in I}$ defined by $U_i\coloneqq V\comp U_i$ for all $i\in I$. Then
$$\begin{equation}
    V\setminus\bigcup_{i\in I}U_i'=\bigcap_{i\in I}V\comp U_i'\cref{\ast}
\end{equation}$$
by the first result. It follows then that
$$\begin{align}
    \bigcup_{i\in I}V\comp U_i&=\bigcup_{i\in I}U_i' && \textrm{Definition of $U_i'$} \\
    &=V\comp\l(V\comp\bigcup_{i\in I}U_i'\r) && \textrm{Double complement} \\
    &=V\comp\l(\bigcap_{i\in I}V\comp U_i'\r) && \ref{\ast} \\
    &=V\comp\l(\bigcap_{i\in I}V\comp\l(V\comp U_i'\r)\r) && \textrm{Definition of $U_i'$} \\
    &=V\comp\bigcap_{i\in I}U_i. && \textrm{Double complement}\qedin
\end{align}$$
