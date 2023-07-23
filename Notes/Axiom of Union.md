<div class="topSpace"></div>

Date Created: 15/01/2022 21:15:56
Tags: #Type/Axiom #Topic/Set_Theory/Later

Constructions: [[Union]]
Generalizations: <i>Not Applicable</i>

Properties: <i>Not Applicable</i>
Sufficiencies: <i>Not Applicable</i>
Equivalences: <i>Not Applicable</i>

``` ad-Axiom
title: Axiom.

Consider the first-order language $\mc{L}$ consisting of one binary relation symbol $\in$. The <b>Axiom of Union</b> is the $\mc{L}$-formula
$$\begin{equation}
    \fa\mc{A}\ex U\fa a\l(a\in U\Leftrightarrow\ex A\in\mc{A}:a\in A\r).
\end{equation}$$

```

<b>Remark.</b> By Extensionality, such a set $U$ is unique and can thus be called the <b>union of $\mc{A}$</b>.<span style="float:right;">$\blacklozenge$</span>

---

<b>Remark.</b> We may weaken this axiom to
$$\begin{equation}
    \fa\mc{A}\ex U':\l(\fa A\in\mc{A},\fa a\in A:a\in U'\r).
\end{equation}$$
Here, $U'$ is no longer the union of $\mc{A}$, but rather a superset thereof. The union $U$ of $\mc{A}$ is then defined as
$$\begin{equation}
    U\coloneqq\l\{a\in U'\st\ex A\in\mc{A}:a\in A\r\}
\end{equation}$$
using Specification.<span style="float:right;">$\blacklozenge$</span>
