<div class="topSpace"></div>

Date Created: 04/02/2022 11:25:15
Tags: #Type/Proposition #Topic/Topology/Later

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\tpl{X,<}$ be a totally ordered set. Then the order topology on $X$, $\mc{T}(<)=\mc{T}\l(\mc{B}\r)$ where $\mc{B}\subseteq\pow\l(X\r)$ is such that
* $\fa a,b\in X:a<b\Rightarrow\l(a,b\r)\in\mc{B}$,
* $\l(\ex a_0\in X:a_0\ \mathit{is\ a\ lower\ bound\ of\ }X\r)\Rightarrow\fa b:\l[a_0,b\r)\in\mc{B}$, and
* $\l(\ex b_0\in X:b_0\ \mathit{is\ an\ upper\ bound\ of\ }X\r)\Rightarrow\fa a:\l(a,b_0\r]\in\mc{B}$,

is a topology on $X$.

```

<i>Proof.</i> It suffices to verify that $\mc{B}$ is a basis for a topology on $X$. To show that $\mc{B}$ covers $X$, there are four cases to consider.
* If there exists a lower bound $a_0\in X$ but not an upper bound, then any other $x\neq a_0$ lies in $\l[a_0,y\r)$ where $y\in X$ is any element greater than $x$. The lower bound itself lies in $\l[a_0,b\r)$ for any $b\in X$.
* Similarly if there exists an upper but not a lower bound in $X$.
* If there exist both a lower bound $a_0\in X$ and an upper bound $b_0\in X$, then they lie in $\l[a_0,b\r)$ and $\l(a,b_0\r]$, respectively, for any $a,b\in X$. Any other $x\in X$ lies in $\l[a_0,y\r)$ where $y\in X$ such that $x<y<b_0$.
* If $X$ is unbounded, then any $x\in X$ lies in $(y,z)$ where $y,z\in X$ and $y<x<z$.

For the basis criterion, it suffices to show that the intersection of any two basis elements is again a basis element (or is empty).
* Neither lower nor upper bounds: $\l(a,b\r)\cap\l(c,d\r)=\l(\max\l\{a,c\r\},\min\l\{b,d\r\}\r)$.
* Lower bound only: $\l[a_0,b\r)\cap\l(c,d\r)=\l(c,\min\l\{b,d\r\}\r)$ and $\l[a_0,b\r)\cap\l[a_0,d\r)=\l[a_0,\min\l\{b,d\r\}\r)$.
* Upper bound only: $\l(a,b_0\r]\cap\l(c,d\r)=\l(\max\l\{a,c\r\},d\r)$ and $\l(a,b_0\r]\cap\l(c,b_0\r]=\l(\max\l\{a,c\r\},b_0\r]$.
* Both lower and upper bounds: $\l[a_0,b\r)\cap\l(a,b_0\r]=\l(\min\l\{a,b\r\},\max\l\{a,b\r\}\r)$.<span style="float:right;">$\blacksquare$</span>
