<div class="topSpace"></div>

Date Created: 02/02/2022 11:09:41
References:
Tags: #Type/Axiom #Topic/Set_Theory/Later/Ordinal

Constructions: [[Set of Natural Numbers]]
Generalizations: <i>Not Applicable</i>

Properties: <i>Not Applicable</i>
Sufficiencies: <i>Not Applicable</i>
Equivalences: <i>Not Applicable</i>

``` ad-Axiom
title: Axiom.

Consider the first-order language $\mc{L}$ consisting of one binary relation symbol $\in$. The <b>Axiom of Infinity</b> is the $\mc{L}$-formula
$$\begin{equation}
    \ex I\l[\l[\ex e\l(\fa x\lnot\l(x\in e\r)\land e\in I\r)\r]\land\l[\fa y\in I:\l(\ex s\l(\fa x\l(x\in s\Leftrightarrow x\in y\lor x=y\r)\land s\in I\r)\r)\r]\r].
\end{equation}$$

```

<b>Remark.</b> Letting $\mc{L}'\coloneqq\mc{L}\cup\l\{\em,S\r\}$ where $\em$ is a constant symbol interpreted as the empty set and $S$ is a function symbol interpreted as the successor, we can rewrite Infinity as the $\mc{L}'$-formula
$$\begin{equation}
    \ex I\l(\em\in I\land\fa y\in I:S\l(y\r)\in I\r).
\end{equation}$$
That is, it is the statement that there exists an inductive set $I$.<span style="float:right;">$\blacklozenge$</span>

---

<b>Remark.</b> This axiom does not directly define the ‘set of all natural numbers’ $\omega$. Rather, it asserts the existence of some inductive set that, by the Principle of Ordinary Induction, contains $\omega$ as a subset.<span style="float:right;">$\blacklozenge$</span>
