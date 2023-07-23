<div class="topSpace"></div>

Date Created: 17/01/2022 13:00:40
Tags: #Type/Definition #Topic/Set_Theory/Later

Types: <i>Not Applicable</i>
Examples: <i>Not Applicable</i>
Constructions: [[Successor]]
Generalizations: <i>Not Applicable</i>

Properties: [[De Morgan's Laws]], [[Image of union is union of images]], [[Preimage of union is union of preimages]]
Sufficiencies: <i>Not Applicable</i>
Equivalences: <i>Not Applicable</i>
Justifications: [[Axiom of Union]], [[Axiom of Extensionality]]

``` ad-Definition
title: Definition.

Let $\mc{A}$ be a set. The <b>union of $\mc{A}$</b> is the set $\bigcup\mc{A}$ whose elements are exactly those that belong to some $A\in\mc{A}$. Formally, $\axiunion$ posits the existence of a set $\bigcup\mc{A}$ such that
$$\begin{equation}
    \fa a\l(a\in\bigcup\mc{A}\Leftrightarrow\ex A\in\mc{A}:a\in A\r).
\end{equation}$$
Such a set $\bigcup\mc{A}$ is unique by $\axiext$.

```

<b>Remark.</b> One can also write the union $\bigcup\mc{A}$ using ‘index’ notation as $\bigcup_{i\in I}A_i$. This is formalized by viewing $\mc{A}$ as an indexed family $\l\{A_i\r\}_{i\in I}$, so the focus shifts from $\mc{A}$ to its elements $A_i$. Note that $\axiunion$ now takes the form
$$\begin{equation}
    \fa a\l(a\in\bigcup_{i\in I}A_i\Leftrightarrow\ex i\in I:a\in A_i\r),
\end{equation}$$
since specifying $i\in I$ uniquely determines $A_i\in\mc{A}$, and conversely too.<span style="float:right;">$\blacklozenge$</span>
