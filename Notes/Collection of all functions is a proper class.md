<div class="topSpace"></div>

Date Created: 28/01/2022 17:27:04
Tags: #Type/Proposition #Topic/Set_Theory/Later

Proved by: [[Collection of all singletons is a proper class]], [[Axiom Schema of Specification]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

The collection of all functions form a proper class.

```

<i>Proof.</i> Suppose, for sake of contradiction, that such a set exists, i.e. $\ex v,\fa f:\l(f\textrm{ is a function }\Rightarrow f\in v\r)$. By Specification, we have
$$\begin{equation}
    \fa z\fa f\l[f\in z\Leftrightarrow f\in v\land\ex x:f=\l\{\tpl{x,x}\r\}\r].
\end{equation}$$
In other words, the set $z$ contains all functions of the form
$$\begin{equation}
    f=\l\{\tpl{x,x}\r\}=\l\{\l\{\l\{x\r\},\l\{x,x\r\}\r\}\r\}=\l\{\l\{\l\{x\r\}\r\}\r\}.
\end{equation}$$
Observe that $\bigcup\bigcup z=\l\{\l\{x\r\}\r\}$; since $x$ is arbitrary, this set is the ‘set of all singletons’ which contradicts the fact that there is none.<span style="float:right;">$\blacksquare$</span>
