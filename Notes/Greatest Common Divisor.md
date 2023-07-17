<div class="topSpace"></div>

Date Created: 14/09/2022 19:47:03
Tags: #Type/Definition #Topic/Ring_Theory

Types: <i>Not Applicable</i>
Examples: <i>Not Applicable</i>
Constructions: [[Content (polynomial)]]
Generalizations: <i>Not Applicable</i>

Properties: <i>Not Applicable</i>
Sufficiencies: [[GCDs exist in UFDs]], [[Bezout's Identity]], [[Euclidean Algorithm]]
Equivalences: <i>Not Applicable</i>
Justifications: [[GCD exists implies unique up to a unit]]

``` ad-Definition
title: Definition.

Let $R$ be a integral domain and fix $a,b\in R\comp\l\{0\r\}$. An element $d\in R\comp\l\{0\r\}$ is said to be a <b>greatest common divisor (GCD) of $a$ and $b$</b> if
* $d$ is a common divisor of $a$ and $b$; that is, if $d\divides a$ and $d\divides b$, and
* for all common divisors $d'$ of $a$ and $b$, $d'\divides d$.

The greatest common divisor of $a$ and $b$ is, up to a unit, unique; write $\gcd\l(a,b\r)\coloneqq d$ and let the <b>GCD ideal of $a$ and $b$</b> be $\gen{d}$.

```

<b>Remark.</b> Rephrasing in terms of ideals, $d$ is a greatest common divisor of $a$ and $b$ iff $\gen{a,b}\subseteq\gen{d}$ and $\gen{d}\subseteq\gen{d'}$ for any ideal $\gen{d'}$ containing $\gen{a,b}$.<span style="float:right;">$\blacklozenge$</span>
