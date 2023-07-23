<div class="topSpace"></div>

Date Created: 12/03/2022 18:33:26
Tags: #Type/Proposition #Topic/Category_Theory/Later

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\cat{C}$, $\cat{D}$, $\cat{E}$, and $\cat{F}$ be categories and consider functors

![[Images/2022-03-13_003038/image.svg|220]]

Then $\l(\ms{H}\circ\ms{G}\r)\circ\ms{F}=\ms{H}\circ\l(\ms{G}\circ\ms{F}\r)$; that is, the diagram

![[Images/2022-03-13_003322/image.svg|220]]

commutes.

```

<i>Proof.</i> We shall prove that $\l[\l(\ms{H}\circ\ms{G}\r)\circ\ms{F}\r]^{\Obj}=\l[\ms{H}\circ\l(\ms{G}\circ\ms{F}\r)\r]^{\Obj}$; the proof for the morphisms part is identical. Take $X\in\Obj\l(\cat{C}\r)$; the result follows by repeated application of the definition:

$\begin{align}
    \l[\l(\ms{H}\circ\ms{G}\r)\circ\ms{F}\r]^{\Obj}\l(X\r)&=\l(\ms{H}\circ\ms{G}\r)^{\Obj}\l[\ms{F}^{\Obj}\l(X\r)\r]\\
    &=\ms{H}^{\Obj}\l(\ms{G}^{\Obj}\l(\ms{F}^{\Obj}\l(X\r)\r)\r)\\
    &=\ms{H}^{\Obj}\l[\l(\ms{G}\circ\ms{F}\r)^{\Obj}\l(X\r)\r]\\
    &=\l[\ms{H}\circ\l(\ms{G}\circ\ms{F}\r)\r]^{\Obj}\l(X\r).\qedin
\end{align}$
