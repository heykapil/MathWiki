<div class="topSpace"></div>

Date Created: 29/01/2022 11:31:28
Tags: #Type/Definition #Topic/Set_Theory/Later

Types: [[Bounded Sequence]], [[Cauchy Sequence]], [[Contractive Sequence]], [[Monotone Sequence]]
Examples: <i>Not Applicable</i>
Constructions: [[Sequential Limits]], [[Subsequences]]
Generalizations: <i>Not Applicable</i>

Properties: <i>Not Applicable</i>
Sufficiencies: <i>Not Applicable</i>
Equivalences: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

``` ad-Definition
title: Definition.

Let $X$ be a set and consider an indexed family $\l\{x_i\r\}_{i\in I}\subseteq X$.
* If $I=\Z$ (or some infinite subset thereof), then $\l\{x_i\r\}_{i\in I}$ is said to be an <b>infinite sequence in $X$</b> and is denoted by either $\tpl{x_i}_{i\in I}$ or $\tpl{x_1,x_2,\dots}$.
* If $I=\l\{1,\dots,n\r\}$ for some $n\in\N$, then $\l\{x_i\r\}_{i\in I}$ is said to be an <b>$n$-tuple in $X$</b> (or a <b>finite sequence in $X$</b>) and is denoted by $\tpl{x_1,\dots,x_n}$.

More generally, let $\l\{X_j\r\}_{j\in J}$ be an indexed family of sets and consider an indexed family $\l\{x_j\r\}_{j\in J}$ where $x_j\in X_j$ for all $j\in J$.
* If $J=\N$, then $\l\{x_j\r\}_{j\in J}$ is said to be an <b>infinite sequence through $\l\{X_j\r\}_{j\in J}$</b>.
* If $J=\l\{1,\dots,n\r\}$ for some $n\in\N$, then $\l\{x_j\r\}_{j\in J}$ is said to be an <b>$n$-tuple through $\l\{X_j\r\}_{j\in J}$</b>.

```

<b>Remark.</b> In other words, infinite sequences and $n$-tuples in $X$ are functions of the form
$$\begin{equation}
    \l[
        \begin{aligned}
            f:\omega&\to X \\
            i&\mapsto x_i\coloneqq f\l(i\r)
        \end{aligned}
    \r]\in X^\omega\ \ \ \ \ \ \ \ \textrm{and}\ \ \ \ \ \ \ \ 
    \l[
        \begin{aligned}
            f:n&\to X \\
            i&\mapsto x_i\coloneqq f\l(i\r)
        \end{aligned}
    \r]\in X^n,
\end{equation}$$
though, in both cases, we usually use $\omega$ as $\N^+$ (as is done above). Similarly, infinite sequences and $n$-tuples through $\l\{X_j\r\}_{j\in J}$ are functions of the form
$$\begin{equation}
    \l[
        \begin{aligned}
            f:\omega&\to\bigcup_{j\in\omega}X_j \\
            j&\mapsto x_j\coloneqq f\l(j\r)
        \end{aligned}
    \r]\in\prod\limits_{j\in\omega}X_j\ \ \ \ \ \ \ \ \textrm{and}\ \ \ \ \ \ \ \ 
    \l[
        \begin{aligned}
            f:n&\to\bigcup_{j\in n}X_j \\
            j&\mapsto x_j\coloneqq f\l(j\r)
        \end{aligned}
    \r]\in\prod_{i=1}^nX_i.\exqedin
\end{equation}$$
