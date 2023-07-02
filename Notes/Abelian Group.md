<div class="topSpace"></div>

Date Created: 04/05/2022 17:13:39
Tags: #Type/Definition #Topic/Group_Theory

Types: <i>Not Applicable</i>
Examples: [[Cyclic Group]]
Constructions: [[Ring]], [[Vector Space]], [[Subgroup Series]]
Generalizations: [[Module]]

Properties: [[Abelian group is simple iff cyclic of prime order]]
Sufficiencies: [[Abelianization]], [[Quotient by center cyclic implies abelian]]
Equivalences: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

``` ad-Definition
title: Definition.

A group $\tpl{G,\ast}$ is said to be <b>abelian</b> if the binary operation $\ast$ commutes.

```

<b>Remark.</b> Every abelian group $M$ can be equipped with a $\Z$-module structure. Indeed, for the $\Z$-module axioms to be satisfied, we need to define, for all $m\in M$, the $\Z$-action on $m$ by $0m\coloneqq0$,
$$\begin{equation}
    nm\coloneqq\underbrace{m+\cdots+m}_{\mathclap{n\textrm{ times}}}
\end{equation}$$
for all $n\in\Z^+$, and $nm\coloneqq\l(-n\r)m$ for every $n\in\Z^-$. Conversely, since every $\Z$-module is an abelian group, we see that the two notions coincide.<span style="float:right;">$\blacklozenge$</span>
