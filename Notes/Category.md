<div class="topSpace"></div>

Date Created: 12/03/2022 17:41:32
Tags: #Type/Definition #Topic/Category_Theory/Later

Types: [[Locally-small Category]], [[Groupoid]]
Examples: <i>Not Applicable</i>
Constructions: [[Morphism (Category Theory)]], [[Functor]], [[Opposite Category]], [[Slice Category]], [[Coslice Category]]
Generalizations: <i>Not Applicable</i>

Properties: <i>Not Applicable</i>
Sufficiencies: <i>Not Applicable</i>
Equivalences: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

``` ad-Definition
title: Definition.

Let $\mb{U}$ be a Grothendieck universe. A <b>$\mb{U}$-category</b> is a quadruple $\cat{C}\coloneqq\tpl{\mc{O},\Hom,\id,\operatorname{comp}}$ consisting of
* a $\mb{U}$-class $\Obj\l(\cat{C}\r)\coloneqq\mc{O}\subseteq\mb{U}$,
* a function $\Hom$ assigning to each $\tpl{X,Y}\in\mc{O}^2$ a $\mb{U}$-class $\Hom\l(X,Y\r)\subseteq\mb{U}$,
* a function $\id$ assigning to each $X\in\mc{O}$ an element $\id_X\coloneqq\id\l(X\r)\in\Hom\l(X,Y\r)$, and
* a function $\operatorname{comp}$ assigning to each $\tpl{X,Y,Z}\in\mc{O}^3$ a function
$$\begin{equation}
    \begin{aligned}
        \circ:\Hom\l(X,Y\r)\times\Hom\l(Y,Z\r)&\to\Hom\l(X,Z\r)\\
        \tpl{f,g}&\mapsto g\circ f\coloneqq\circ\tpl{f,g},
    \end{aligned}
\end{equation}$$

such that, for all $X,Y,Z,W\in\mc{O}$:
* (Associativity)$\bf{.}$ For all $f\in\Hom\l(X,Y\r)$, $g\in\Hom\l(Y,Z\r)$, and $h\in\Hom\l(Z,W\r)$, the following diagram commutes.
![[Images/2022-02-21_142913/image.svg|230]]

* (Unit)$\bf{.}$ For all $f\in\Hom\l(X,Y\r)$, the following diagram commutes.
![[Images/2022-02-09_213021/image.svg|230]]
* (Disjoint)$\bf{.}$ If $X\neq Z$ or $Y\neq W$, then $\Hom\l(X,Y\r)\cap\Hom\l(Z,W\r)=\em$.

```

<b>Remark.</b> The last axiom can be ‘forced’ to hold since one can replace morphisms $f\in\Hom\l(X,Y\r)$ with the triple $\tpl{f,X,Y}$; this is done, for instance, in $\catset$.<span style="float:right;">$\blacklozenge$</span>
